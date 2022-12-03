<template>
    <section>
        <div class="container">
            <h5>CUSTOMERS TESTIMONIALS</h5>
            <div class="title">
                <span class="title-1">Trusted</span>
                <span class="title-2">Feedback</span>
            </div>
            <p>We work with innovative methodologies to ensure that the entire reformatting process is done from start to finish as planned.</p>
        </div>
        
        <div class="card-box">
            <div class="card">
                <img src="../assets/img/logo-1.png" alt="">
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Atque expedita ea facere, ab consequatur pariatur mollitia, nam earum amet nihil voluptatem veritatis quaerat.</p>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                <font-awesome-icon icon="fa-solid fa-quote-right" />
            </div>
            <div class="card">
                <img src="../assets/img/logo-2.png" alt="">
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Atque expedita ea facere, ab consequatur pariatur mollitia, nam earum amet nihil voluptatem veritatis quaerat.</p>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                <font-awesome-icon icon="fa-solid fa-quote-right" />
            </div>
            <div class="card">
                <img src="../assets/img/logo-3.png" alt="">
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Atque expedita ea facere, ab consequatur pariatur mollitia, nam earum amet nihil voluptatem veritatis quaerat.</p>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                <font-awesome-icon icon="fa-solid fa-quote-right" />
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'TestimonialSection',
    }
</script>

<style lang="scss" scoped>
    
    section{
        background-color: #EEF4ED;
        padding: 100px 0;

        .container{
            width: 35%;
            margin-inline: auto;
            text-align: center;
            margin-bottom: 50px;

            h5{
            color: #00A7A6;
            }

            .title{
                font-size: 2.7rem;
                font-weight: 800;
                margin: 30px 0;

                .title-2{
                    margin-left: 10px;
                    padding: 0 10px;
                    background-color: #CCE3DE;
                    color: #058283;
                    border-radius: 5px;
                }
            }

            p{
                color: grey;
            }
        }

        .card-box{
            width: 60%;
            margin-inline: auto;
            display: flex;
            gap: 40px;

            .card{
                width: calc((100% / 3 ) - 20px );
                background-color: white;
                border-radius: 10px;
                padding: 40px 30px;
                position: relative;

                img{
                    height: 25px;
                }

                p:last-child{
                    width: 80%;
                }

                p{
                    color: grey;
                    margin-top: 20px;
                }

                .fa-quote-right{
                    position: absolute;
                    bottom: 20px;
                    right: 20px;
                    font-size: 2rem;
                    color: lightgrey;
                }
            }
        }

    }

</style>