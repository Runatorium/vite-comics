<script>
export default{
    name: 'JumboTron',
}

</script>

<template>
    <div id="Jumbotron">
    </div>
    <div id="button">
        <h3>Current Series</h3>
    </div>
</template>







<style scoped>
#Jumbotron{
    width: 100%;
    justify-content: center;
    background-image: url(../../img/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 450px;
}

h3{
    position: absolute;
    display: inline;
    padding: 10px 40px;
    left: 225px;
    top: 525px;
    background-color: rgb(8, 103, 197);
    color: white;
}

</style>