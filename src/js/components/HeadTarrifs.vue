<template>
    <div class="head">
        <div class="lead">
            <div>
                <h1>Cardio <br>Excercise</h1>
                <p>Огромный выбор материалов о здоровье и фитнесе, полезных рецептов и историй преображения, которые помогут вам привести себя в форму и оставаться в форме!</p>
                <div class="lead_buttons">
                    <button>Присоединяйтесь</button>
                    <img src="/img/companies.png" alt="Workout">
                </div>
            </div>
            <div>
                <img src="/img/lead2.png" alt="Workout">
                <div class="lead_info">
                    <div class="lead_info_km">
                        <i class="fa-solid fa-person-running"></i>
                        <span>4.95</span> km
                    </div>
                    <div class="lead_info_training">
                        <i class="fa-solid fa-play"></i>
                        <span>350+</span>
                        Тренировок
                    </div>
                    <div class="lead_info_videos">
                        <span>500+</span>
                        Бесплатных видео
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default{
   
}
</script>

<style lang="scss" scoped>
.head{
    margin-top: 70px;
    
    @media (min-width: 1024px)  {
    overflow: hidden;
    height: 800px;
    }
}

.lead {
    margin-top: 20px;
    display: flex;
    position: relative;
    h1 {
        font-size: 12em;
        line-height: 170px;
        word-spacing: -2px;
        @media (min-width: 1500px) {
            font-size: 12em;
            line-height: 170px;
        }
        @media (max-width: 1500px) and (min-width: 1300px) {
            font-size: 11em;
            line-height: 160px;
        }
        @media (max-width: 1300px) and (min-width: 650px) {
            font-size: 8.5em;
            line-height: 150px;
        }
        @media (max-width: 650px) and (min-width: 450px)  {
            font-size: 5.5em;
            line-height: 110px;
        }
        @media (max-width: 450px)  {
            font-size: 3.8em;
            line-height: 90px;
        }
        
    }
    p {
        color: #868686;
        
        margin: 20px 0;
        @media (min-width: 650px)  {
            width: 600px;
            }
    }
    button {
        background: #e6533c;
        padding: 20px;
        
        font-weight: 600;
        font-size: 1.02em;
        color: #fff;
        border: 0;
        cursor: pointer;
        border-radius: 10px;
        margin-top: 30px;
        transition: transform 500ms ease;
       
        &:hover {
            transform: translatey(-7px);
        }
    }

    > div:first-of-type img {
        display: block;
        max-width: 100%;
        margin-top: 70px;
    }

    > div:last-of-type{

        @media (max-width: 1024px)  {
                display: none;
            }
        img {
            position: relative;
            

            @media (min-width: 1500px)  {
                top: 80px;
                right: 80px;
            }
            @media (max-width: 1500px) and (min-width: 1300px) {
                transform: scale(0.85);
                top: 40px;
                right: 100px;
            }
            @media (max-width: 1300px)  {
                transform: scale(0.7);
                top: 40px;
                right: 120px;
            }
        }

        .lead_info {
            position: absolute;
            top: 0;
            right: 0;

            @mixin info-block{
                border-radius: 20px;
                padding: 20px 30px;
                width: 110px;
                font-size: 0.7em;
                margin-bottom: 25px;
                position: relative;

                span {
                    font-weight: 600;
                    color: #fff;
                }

                i {
                    padding: 10px;
                    border-radius: 50%;
                    color: #fff;
                    font-size: 1.3em;
                    text-align: center;
                    width: 14px;
                    height: 14px;
                    line-height: 14px;
                }
            }
            .lead_info_km {
                @include info-block;
                background: #ef8964;
                color: #efcaba;
                right: 80px;
                top: 40px;

                span {
                    font-size: 2.7em;
                    margin-right: 4px;
                }

                i {
                    display: block;
                    background: #efa082; 
                }
            }
            .lead_info_training {
                @include info-block;
                background: #303030;
                color: #ACABA8;
                top: 300px;
                @media (min-width: 1450px){
                right: 480px;
                }
                @media (max-width: 1450px) and (min-width: 1100px){
                right: 350px;
                }
                @media (max-width: 1100px){
                right: 250px;
                }
                span {
                    font-size: 1.7em;

                }

                i {
                    background: #ef8963;
                    float: left;
                    position: relative;
                    top: 8px;
                    margin-right: 7px;
                }
            }
            .lead_info_videos {
                @include info-block;
                background: #7a29dc;
                color: #c6a8e4;
                right:  70px;
                top: 300px;

                span {
                    font-size: 2.5em;
                }
            }
        }
    }
}
</style>