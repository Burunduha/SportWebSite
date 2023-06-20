<template>
    <div>
        <div class="blocks">
            <div>
                <h2>Тренируйтесь дома</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione hic asperiores eligendi sed placeat qui, repellat laboriosam veritatis consectetur corporis quia. Et fugiat, deleniti dolorem quis praesentium at maiores vel, eos excepturi numquam quae corrupti velit sunt earum, ipsum voluptas harum inventore reiciendis maxime incidunt dolor. Suscipit facere laboriosam odit!</p>
                <span><a href="">Больше</a><i class="fas fa-arrow-right"></i></span>
            </div>
            <div>
                <img src="/img/info-1.png" alt="Workout">
            </div>
        </div> 
        <div class="blocks">
            <div>
                <img src="/img/info-2.png" alt="Workout">
            </div>
            <div>
                <h2>Получите еще <br>больше полезного <br>контента</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis minus fuga facilis explicabo nam. Suscipit provident culpa, beatae ipsam praesentium veniam quo, laboriosam eos quaerat porro vero nobis deserunt? Et deleniti error, nulla deserunt quisquam sit, ipsa dolorem ipsam id reprehenderit nihil. Assumenda eveniet in nihil rem, expedita dolore nostrum!</p>
                <span><a href="">Больше</a><i class="fas fa-arrow-right"></i></span>
            </div>
            
        </div> 
    </div>
</template>

<script>

export default {

}
</script>

<style lang="scss" scoped>
 .blocks {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin-top: 80px;

    @media (max-width: 1100px){
        flex-direction: column;
    }

    > div {
        
        @media (min-width: 900px){
            width: 50%;
    }

        h2 {
            margin-bottom: 30px;
            font-size: 2.2em;
        }

        p {
            color: #9b9a97;
            max-width: 450px;
            margin-bottom: 20px;
        }
        span {
            a {
                color: #0070c9;
            }

            i {
                margin-left: 15px;
                font-size: 1.2em;
            }
        }
        
        img {
            max-width: 90%;

            @media (max-width: 1100px) {
                &:first-of-type {
                    margin-top: 30px;
                }
            }
        }
    }
 }
</style>