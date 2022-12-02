<template>
    <header>
        <div class="banner">
            <div class="container">
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
        
    </header>
</template>

<script>
    export default {
        name: 'HeaderComp'
    }
</script>

<style lang="scss" scoped>
    .banner{
        background-color: #21333E;
        padding: 10px 0;
        .container{
            width: 60%;
            margin-inline: auto;
            color: lightgrey;
            display: flex;
            justify-content: space-between;
            font-size: 0.9rem;
        }
    }

    a{
        text-decoration: none;
        color: inherit;
        margin-right: 30px;
    }

</style>