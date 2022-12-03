<template>
    <section>
        <div class="container">
            <h5>WE DO MORE FOR EVERYONE</h5>
            <div class="title">
                <span class="title-1">Actions &</span>
                <span class="title-2">Projects</span>
            </div>
            <ul>
                <li>ALL</li>
                <li>INSTITUTIONAL</li>
                <li>SOCIAL</li>
                <li>EVENTS</li>
                <li>INNOVATION</li>
                <li>ENVIRORMENT</li>
                <li>TECHNOLOGY</li>
            </ul>
            <div class="card-box">
                <div class="card" v-for="(elem, index) in cards" :key="index">
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
                
                li:first-child{
                        font-weight: 600;
                        background-color: #0E272D;
                    }

                li{
                    list-style: none;
                    padding: 7px 5px;
                    border-radius: 5px;
                }
            }

            .card-box{
                display: flex;
                flex-wrap: wrap;
                justify-content: center;
                gap: 20px;
                margin-top: 50px;

                .card{
                    width: calc(100% / 3 - 20px);
                    aspect-ratio: 1/1;
                    border-radius: 10px;
                    position: relative;
                    display: flex;
                    justify-content: center;
                    align-items: flex-end;
                    
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

</style>