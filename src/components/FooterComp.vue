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
                    color: white;
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