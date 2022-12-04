<template>
    <section>
        <div class="container">
            <div class="card">
                <div class="img-box">
                    <font-awesome-icon icon="fa-solid fa-user-group" />
                </div>
                <div class="card-title">
                    <span>Human Capital</span>
                </div>
                <div class="card-info">
                    <span>Humanizing business: Harness the power of technology to improve the way people work.</span>
                </div>
            </div>

            <div class="card">
                <div class="img-box">
                    <font-awesome-icon icon="fa-solid fa-chart-pie" />
                </div>
                <div class="card-title">
                    <span>Core Business</span>
                </div>
                <div class="card-info">
                    <span>It takes innovative approaches to transform, modernize, and run existing platforms.</span>
                </div>
            </div>

            <div class="card">
                <div class="img-box">
                    <font-awesome-icon icon="fa-solid fa-gauge-high" />
                </div>
                <div class="card-title">
                    <span>Performance</span>
                </div>
                <div class="card-info">
                    <span>Achieving maximum impact and value from investments in finance and supply chain.</span>
                </div>
            </div>

        </div> 
    </section>
</template>

<script>
    export default {
        name: 'ToolSection',
    }
</script>

<style lang="scss" scoped>
    
    section{
        
        background-color: #EEF4ED;
        padding: 100px 0 150px 0;
        
        .container{
            width: 60%;
            margin-inline: auto;
            display: flex;
            justify-content: space-between;
            gap: 50px;

            .card{
                width: calc(100% / 3);
                padding: 40px;
                background-color: white;
                border-radius: 10px;

                .img-box{
                    width: 50px;
                    height: 50px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    background-color: #DAECED;
                    border-radius: 50%;
                    color: #058283;
                    font-size: 1.4rem;
                }

                .card-title{
                    margin-top: 20px;
                    font-size: 1.2rem;
                    font-weight: 600;
                }

                .card-info{
                    margin-top: 20px;
                    color: grey;
                }
            }
        }
    }

</style>