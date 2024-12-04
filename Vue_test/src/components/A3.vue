<template>
    <div class="content">
        <h1>欢迎来到山东大学主页</h1>
        <p></p>
    <div class="background-image"></div>
    </div>
</template>

<style scoped>
.content{
    display: flex;
    flex-direction: column;
    justify-content: center;
    flex-grow: 1;
    padding: 30px;
    
}
h1{
    background-color: #5cb9d8;
    color: rgb(12, 55, 92);
    padding: 10px 20px;
    margin: 0;
    text-align: center;
}
.background-image{
    width: 100%;
    height: 1000px;
    background-image: url('@/assets/SDU.jpg');
    background-size: cover;
    background-position: center;
}

</style>