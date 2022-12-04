<template>
    <section>
        <div class="dots-img-1">
            <div class="dot-box" v-for="(elem, index) in 36" :key="index">
                <div class="dot"></div>
            </div> 
        </div>
        <div class="dots-img-2">
            <div class="dot-box" v-for="(elem, index) in 36" :key="index">
                <div class="dot"></div>
            </div>
        </div>
        <div class="network-container">
            <div class="network-box">
                <h5>ABOUT THE NETWORK</h5>
                <div class="title">
                    <span class="title-1">The</span>
                    <span class="title-2">Company</span>
                </div>
                <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia sed ipsam ratione ea? Nesciunt, eos totam inventore nam similique quidem?
                </p>
                <div class="card-box">
                    <div class="card">
                        <div class="counter">
                            <span>0</span>
                        </div>
                        <div class="target">
                            <span>Employees</span>
                        </div>
                        <div class="card-info">
                            <span>Lorem ipsum dolor sit amet.</span>
                        </div>
                    </div>
                    <div class="card">
                        <div class="counter">
                            <span>0</span>
                        </div>
                        <div class="target">
                            <span>Partners</span>
                        </div>
                        <div class="card-info">
                            <span>Lorem ipsum dolor sit amet.</span>
                        </div>
                    </div>
                    <div class="card">
                        <div class="counter">
                            <span>0</span>
                        </div>
                        <div class="target">
                            <span>Customers</span>
                        </div>
                        <div class="card-info">
                            <span>Lorem ipsum dolor sit amet.</span>
                        </div>
                    </div>
                </div>
                <div class="btn-box">
                    <a href="#"><div class="btn btn-1">GET IN TOUCH</div></a>
                    <a href="#"><div class="btn btn-2">READ MORE</div></a>
                </div> 
            </div>
        </div>
        <div class="img-box">

        </div>
    </section>
</template>

<script>
    export default {
        name: 'NetworkSection',
    }
</script>

<style lang="scss" scoped>
    
    section{
        display: flex;
        position: relative;

        .dots-img-1{
            position: absolute;
            top: -40px;
            left: 50%;
            display: flex;
            flex-wrap: wrap;
            width: 180px;
            height: 80px;
            transform: translateX(-50%);
        }

        .dots-img-2{
            position: absolute;
            bottom: -40px;
            left: 50%;
            display: flex;
            flex-wrap: wrap;
            width: 180px;
            height: 80px;
            transform: translateX(-50%);
        }

        .dot-box{
                display: flex;
                justify-content: center;
                align-items: center;
                width: calc(100% / 9);
                height: calc(100% / 4);

                .dot{
                    width: 40%;
                    aspect-ratio: 1/1;
                    border-radius: 50%;
                    background-color: #00A6A6;
                    opacity: 0.3;
                }
        }

        .network-container{
            width: 50%;

            .network-box{
                width: 60%;
                margin-left: auto;
                height: 100%;
                padding: 100px 0;
                padding-right: 50px;

                h5{
                    color: #00A7A6;
                }

                .title{
                    font-size: 2.7rem;
                    font-weight: 800;
                    margin: 30px 0;

                    .title-1{
                        margin-right: 10px;
                        padding: 5px 10px;
                        background-color: #DAECED;
                        color: #058283;
                        border-radius: 5px;
                    }
                }

                p{
                    color: grey;
                    line-height: 1.3rem;
                    margin-bottom: 50px;
                }

                .card-box{
                    display: flex;
                    gap: 20px;
                    margin-bottom: 50px;

                    .card{
                        width: calc(100% / 3);
                        text-align: center;

                        .counter {
                            color: #00A6A6;
                            font-size: 2rem;
                            font-weight: 800;
                        }

                        .target{
                            font-size: 1.5rem;
                            font-weight: 600;
                        }

                        .card-info{
                            color: grey;
                        }

                        *{
                            padding-bottom: 20px;
                        }
                    }

                    
                }
                
                .btn-box{

                        .btn-1{
                            background-color: #058283;
                            margin-right: 20px;
                            font-size: 0.9rem;
                            color: white;
                        }

                        .btn-2{
                            border: 2px solid #058283;
                            font-size: 0.9rem;
                            color: #058283;
                        }

                    }

            }

        }

        .img-box{
            width: 50%;
            background-image: url(../assets/img/about-5.jpg);
            background-size: cover;
            background-repeat: no-repeat;
        }

        .btn{
            padding: 15px 30px;
            border-radius: 5px;
            display: inline-block;
        }

    }

</style>