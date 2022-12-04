<template>
    <section>
        <div class="container">
            <h5>WE DO MORE FOR EVERYONE</h5>
            <div class="title">
                <span class="title-1">Actions &</span>
                <span class="title-2">Projects</span>
            </div>
            <ul>
                <li v-for="(elem, index) in projectsList" :key="index" @click="filterCards(elem)" :class="(activeFilter == elem) ? 'active' : ''">{{elem.toUpperCase()}}</li>
            </ul>
            <div class="card-box">
                <div class="alert-box" v-if="this.filteredArray == ''">
                    <span>No projects found in this section.</span>
                </div>
                <div class="card" v-for="(elem, index) in filteredArray" :key="index">
                    <img :src="require(`../assets/img/${elem.imgPath}`)" alt="">
                    <span>{{elem.text}}</span>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'ProjectSection',
        props: {
            cards: Array,
        },

        data(){
            return{
                projectsList: [
                    'all',
                    'institutional',
                    'social',
                    'events',
                    'innovation',
                    'environment',
                    'technology'
                ],

                activeFilter: 'all',
                filteredArray:  [],
            }
        },

        mounted(){
            this.filterCards(this.activeFilter)
        },

        methods: {
            filterCards(elem){
                this.filteredArray = [];
                this.activeFilter = elem;
                if(this.activeFilter == 'all'){
                    this.filteredArray = this.cards;
                }else{
                    this.cards.forEach(card =>{
                        if(card.category == elem){
                            this.filteredArray.push(card)
                        }
                    })
                }        
            }
        }
    }
</script>

<style lang="scss" scoped>
    
    section{

        background-color: #111117;
        text-align: center;
        padding: 100px 0;
        
        .container{
            width: 60%;
            margin-inline: auto;

            h5{
            color: #00A7A6;
            }

            .title{
                font-size: 2.7rem;
                font-weight: 800;
                margin: 30px 0;
                color: white;

                .title-2{
                    margin-left: 10px;
                    padding: 0 10px;
                    background-color: #0E272D;
                    border-radius: 5px;
                }
            }

            ul{
                display: flex;
                color: white;
                justify-content: center;
                gap: 40px;
                font-size: 0.9rem;
                padding-top: 20px;

                li{
                    list-style: none;
                    padding: 7px 5px;
                    border-radius: 5px;

                    &:hover{
                        scale: 1.1;
                        cursor: pointer;
                    }
                }
            }

            .card-box{
                display: flex;
                flex-wrap: wrap;
                gap: 30px;
                margin-top: 50px;
                justify-content: center;

                .alert-box{
                    width: calc(100% / 3 - 20px);
                    aspect-ratio: 1/1;
                    border-radius: 10px;
                    display: flex;
                    justify-content: center;
                    align-items: center;

                    span{
                        color: white;
                        font-size: 1.5rem;
                        font-weight: 600;
                        padding: 20px;
                    }
                }

                .card{
                    width: calc(100% / 3 - 20px);
                    aspect-ratio: 1/1;
                    border-radius: 10px;
                    position: relative;
                    display: flex;
                    justify-content: center;
                    align-items: flex-end;
                    overflow: hidden;

                    &:hover{
                        scale: 1.1;
                        transition: 0.5s;
                        cursor: pointer;

                        img{
                            scale: 1.3;
                            transition: 2s;
                        }
                    }
                    
                    img{
                        position: absolute;
                        top: 0;
                        left: 0;
                        right: 0;
                        bottom: 0;
                        width: 100%;
                        border-radius: 10px;
                        // aspect-ratio: 1/1;
                        z-index: 0;
                        filter: brightness(0.6);
                    }

                    span{
                        color: white;
                        font-size: 1.5rem;
                        font-weight: 600;
                        position: relative;
                        z-index: 2;
                        padding: 20px;
                        margin-bottom: 30px;
                    }
                }
            }
        }  
    }

    .active{
        font-weight: 600;
        background-color: #0E272D;
    }

</style>