<script>

    export default{
        name: 'TheFooter',
        footerData:[
        {
          dcComics:[
            Characters,
            Comics,
            Movies,
            Tv,
            Games,
            Videos,
            News,
          ]
        }
      ]
    }

</script>

<template>
    <footer class="d-flex">
        <div id="leftcontainer">
            <div>
                <ul>
                    <li id="title">Dc Comics</li>
                    <li v-for="(data, i) in footerData" :key="i">{{footerData.dcComics[i]}}</li>
                </ul>
                <ul></ul>
            </div>
            <div>
                <ul></ul>
            </div>
            <div>
                <ul></ul>
            </div>
        </div>
        <div id="rightcontainer">
            <img src="../../img/dc-logo-bg.png" alt="">
        </div>
    </footer>

</template>

<style scoped>

footer{
    justify-content: center;
    background-image: url(../../img/footer-bg.jpg);
}  
ul{
    list-style: none;
}
#rightcontainer{
        border-style: dashed; /*Debug Feature*/
        border-color: aqua; /*Debug Feature*/
    }

#leftcontainer{
        border-style: dashed; /*Debug Feature*/
        border-color: aqua; /*Debug Feature*/
    }
</style>