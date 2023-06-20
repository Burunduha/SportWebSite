<template>
    <div class="wrapper">
        <div class="container">
            <router-view></router-view>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss">
$mainColor: #000000;
$textColor: #fff;
$additionColor: #25ab75;

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

::selection {
    background: $additionColor;
}

*{
    margin: 0;
    padding: 0;
}
body {
    background: $mainColor;
    color: $textColor;
    font-family: 'Poppins', sans-serif;
    font-weight: 400;
    font-size: 1em;
}

.wrapper {overflow: hidden;}

a {
    color: #ABABAB;
    text-decoration: none;
    &:hover {
        color: #c7c7c7
    }
}

.container {

    @media(min-width: 1500px){
        width: 1360px;
        margin: 0 auto;
    }
    @media(max-width: 1500px) and (min-width: 900px){
        width: 80%;
        margin: 0 10%;
    }
    @media(max-width: 900px){
        width: 90%;
        margin: 0 5%;
    }
}
</style>