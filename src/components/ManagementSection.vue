<template>
    <section>
        <div class="top-section">
            <h5>HOW IT WORKS IN PRACTICE</h5>
            <div class="title">
                <span class="title-1">Process</span>
                <span class="title-2">Management</span>
            </div>
            <p>We work with innovative methodologies to ensure that the entire reformatting process is done from start to finish as planned.</p>
        </div>
        <div class="blue-line"></div>
        <div class="bottom-section">
            
            <div class="box">
                <div class="number-box">
                    <span class="number">01</span>
                </div>
                <h2>Collection of information</h2>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>
            
            <div class="box">
                <div class="number-box">
                    <span class="number">02</span>
                </div>
                <h2>Strategic planning</h2>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>

            <div class="box">
                <div class="number-box">
                    <span class="number">03</span>
                </div>
                <h2>Assignment of responsibilities</h2>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>

            <div class="box">
                <div class="number-box">
                    <span class="number">04</span>
                </div>
                <h2>Formatting Process</h2>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>

            <div class="box">
                <div class="number-box">
                    <span class="number">05</span>
                </div>
                <h2>Continuity formalization</h2>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>

            

        </div>
    </section>
</template>

<script>
    export default {
        name: 'ManagementSection',
    }
</script>

<style lang="scss" scoped>

section{
    
    padding: 100px 0;

    .top-section{

        width: 35%;
        text-align: center;
        margin-inline: auto;
        padding-bottom: 70px;
    
        h5{
            color: #00A7A6;
        }

        .title{
            font-size: 2.7rem;
            font-weight: 800;
            margin: 30px 0;

            .title-1{
                margin-right: 10px;
                padding: 0 10px;
                background-color: #DAECED;
                color: #058283;
                border-radius: 5px;
            }
        }

        p{
            color: grey;
        }
    }

    .blue-line{
        width: 100%;
        background-color: #DAECED;
        height: 5px;
    }

    .bottom-section{
        width: 80%;
        margin-inline: auto;
        display: flex;
        gap: 40px;
        position: relative;
        top: -20px;

        .box{
            width: calc( 100% / 5 );
            height: 200px;
            justify-content: flex-start;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;

            > *{
                margin-bottom: 20px;
            }

            .number-box{
                width: 40px;
                height: 40px;
                display: flex;
                justify-content: center;
                align-items: center;
                background-color: #DAECED;
                border-radius: 50%;
                color: #058283;
                font-size: 1.2rem;
                font-weight: 600;
            }

            p{
                color: grey;
            }
        }
    }

}
    

</style>