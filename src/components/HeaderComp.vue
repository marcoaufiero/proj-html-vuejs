<template>
    <header>
        <div class="banner">
            <div class="banner-box container-60">
                <div>
                    <font-awesome-icon icon="fa-solid fa-clock" />
                    <span> Open Hours: Mon - Sat / 9:00 - 18:00</span>
                </div>
                <div>
                    <a href="#">
                        <font-awesome-icon icon="fa-solid fa-phone" />
                        <span> +1 (305) 1234-5678</span>
                    </a>
                    <a href="#">
                        <font-awesome-icon icon="fa-solid fa-envelope" />
                        <span> hello@example.com</span>
                    </a>
                    <a href="#">
                        <font-awesome-icon icon="fa-brands fa-facebook-f" />
                    </a>
                    <a href="#">
                        <font-awesome-icon icon="fa-brands fa-twitter" />
                    </a>
                    <a href="#">
                        <font-awesome-icon icon="fa-brands fa-linkedin-in" />
                    </a>
                </div>
            </div>
        </div>
        
        <div class="hero">
            <div class="container-60">
                
                <nav>
                    <a href="#">
                        <span class="title-1">N E X</span>
                        <span class="title-2">G E N</span>
                    </a>
                    <ul>
                        <li v-for="(elem, index) in info" :key="index"><a :href="elem.href">{{elem.name}}</a></li>
                        <li><a href="#"><font-awesome-icon icon="fa-regular fa-user" /></a></li>
                        <a href="#"><li class="btn nav-btn">GET IN TOUCH</li></a>
                    </ul>
                </nav>
            
                <div class="intro">
                    <h4>HUMAN RESOURCES</h4>
                    <div id="title">
                        <h1>Get More</h1>
                        <h1>Productivity</h1>
                        <div class="blue-bg"></div>
                    </div>
                    <span class="intro-info">
                        Planning, recruitment and selection process and performance evaluation of employees.
                    </span>
                    <div class="intro-btn">
                        <a href="#"><div class="btn intro-btn-1">GET IN TOUCH</div></a>
                        <a href="#"><div class="btn intro-btn-2">READ MORE</div></a>
                    </div>
                    
                </div>
            
            </div>
        </div>

        
        
    </header>
</template>

<script>
    export default {
        name: 'HeaderComp',
        props:{
            info: Array,
        }
           
    }
</script>

<style lang="scss" scoped>
    
    .banner{
        background-color: #21333E;
        padding: 10px 0;
        .banner-box{
            color: lightgrey;
            display: flex;
            justify-content: space-between;
            font-size: 0.9rem;

            a{
                text-decoration: none;
                color: inherit;
                margin-left: 30px;
            }
        }
    }

    .hero{
        position: relative; 
        width: 100%;

        ::after{
            content: "";
            background-image: url(../assets/img/bg-4.jpg);
            background-size: cover;
            background-repeat: no-repeat;
            filter: brightness(0.6);
            position: absolute;
            top: 0px;
            right: 0px;
            bottom: 0px;
            left: 0px;
            z-index: -1;
        }

        nav{
            color: white;
            padding-top: 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            
            .title-1{
                font-size: 1.3rem;
                font-weight: 600;
                background-color: #14312F;
                color: #00A7A7;
                padding: 10px 3px 10px 20px;
                margin-right: 3px;
                border-top-left-radius: 20px;
                border-bottom-left-radius: 20px;
            }

            .title-2{
                font-size: 1.3rem;
                font-weight: 600;
                color: lightgrey;
            }

            ul{

                display: flex;
                align-items: center;

                .nav-btn{
                    background-color: #058283;
                }

                >li:hover{
                    box-shadow: 0 2px 0 white;
                }

                li{
                    margin-left: 30px;
                    list-style: none;
                    font-weight: 600;
                }

                .nav-btn:hover{
                    background-color: #078f8f;
                }

            }

            a{
                text-decoration: none;
                color: inherit;
            }
        }

        .intro{
            
            padding: 150px 0 250px 0;
            width: 50%;

            h4{
                color: #00A7A6;
            }

            #title{
                font-size: 2rem;
                color: white;
                margin: 20px 0;
            }

            .intro-info{
                font-size: 1.5rem;
                color: rgb(176, 176, 176);
            }
            
            .intro-btn{
                margin-top: 30px;

                .intro-btn-1{
                    background-color: #058283;
                    margin-right: 20px;
                    font-size: 0.9rem;

                    &:hover{
                        background-color: #078f8f;
                    }
                }

                .intro-btn-2{
                    border: 2px solid #058283;
                    font-size: 0.9rem;

                    &:hover{
                        background-color: #078f8f;
                    }
                }
            }  
        }
    }

    .btn{
        padding: 15px 30px;
        border-radius: 5px;
        display: inline-block;
        color: white;
    }

    .container-60{
        width: 60%;
        margin-inline: auto;
    }

    

</style>