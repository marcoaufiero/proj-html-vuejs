<template>
    <footer>
        <div class="footer-top">
            <div class="container-1">
                
                <div class="left-section">
                    <h5>SEND MESSAGE</h5>
                    <div class="title">
                        <span class="title-1">Get in</span>
                        <span class="title-2">Touch</span>
                    </div>
                    <p>We will respond to your message as soon as possible.</p>
                    
                    <form action="">
                        
                        <input type="text" placeholder="Name">
                        <input type="mail" name="" id="" placeholder="Email">
                        <input type="tel" placeholder="Phone">
                        <select name="" id="">
                            <option value="default">More info</option>
                            <option value=""></option>
                            <option value=""></option>
                        </select>
                        <textarea name="" id="" cols="30" rows="10" placeholder="Message"></textarea>
                        <button>SEND</button>

                    </form>
                </div>
                
                <div class="right-section">
                    <h2>Example Inc.</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <p>Praesent diam Iacus, dapibus sed imperdiet consectetur.</p>
                    <div>
                        <div class="i-block">
                            <div class="img-box"><font-awesome-icon icon="fa-solid fa-phone" /></div>
                        </div>
                        <div class="i-block">
                            <span>+1 (305) 1234-5678</span>
                        </div>
                    </div>
                    <div>
                        <div class="i-block">
                            <div class="img-box"><font-awesome-icon icon="fa-solid fa-envelope" /></div>
                        </div>
                        <div class="i-block">
                            <span>hello@example.com</span>
                        </div>
                    </div>
                    <div>
                        <div class="i-block">
                            <div class="img-box"><font-awesome-icon icon="fa-solid fa-location-dot" /></div>
                        </div>
                        <div class="i-block">
                            <span>Main Avenue, 987</span>
                        </div>
                    </div>
                    <div class="btn">VIEW MAP</div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">

            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        name: 'FooterComp'
    }
</script>

<style lang="scss" scoped>
    
    .footer-top{
        background-color: #111117;

        .container-1{
            width: 60%;
            display: flex;
            margin-inline: auto;
            padding: 100px 0;

            .left-section{
                width: 60%;

                h5{
                    color: #00A7A6;;
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

                p{
                    color: rgb(158, 158, 158);
                }

                form{
                    margin-top: 50px;
                    display: flex;
                    flex-wrap: wrap;
                    gap: 20px;

                    >*{
                        background-color: #1D1D23;
                        border: none;
                        border-radius: 5px;
                        color: grey;
                        font-size: 1.1rem;
                    }

                    >*::placeholder{
                        color: grey;
                    }

                    input, select{
                        width: calc(100% / 2 - 10px );
                        padding: 15px;
                    }

                    textarea{
                        width: 100%;
                        padding: 15px;
                        resize: none;
                    }

                    button{
                        color: white;
                        background-color: #058283;
                        border-radius: 3px;
                        padding: 10px 15px;
                    }
                }  
            }

            .right-section{
                width: 40%;
                padding-left: 70px;

                >*{
                    margin-bottom: 30px;
                }

                h2{
                    color: white
                }

                p{
                    color: rgb(158, 158, 158);
                    font-size: 1.1rem;
                    line-height: 1.5rem;
                }
                
                .i-block{
                    display: inline-block;
                    vertical-align: middle;
                }

                .img-box{
                    width: 50px;
                    height: 50px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    background-color: #0F2128;
                    border-radius: 50%;
                    color: #058283;
                    font-size: 1.4rem;
                }

                span{
                    color: #058283;
                    font-size: 1.1rem;
                    margin-left: 10px;
                }

                .btn{
                    border: 1px solid #00A7A6;
                    padding: 10px 20px;
                    color: white;
                    border-radius: 3px;
                    display: inline-block;
                }
            }
        
        }
    }

    .footer-bottom{
        background-color: #0D0D11;

        .container-2{
            width: 60%;
        }
    }

   

</style>