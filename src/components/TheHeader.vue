
<script>

export default{
    name: 'TheHeader',

    data() {

    return {
      navData: [
        {
          href: "#home",
          text: "Characters",      
        },
        {
          href: "#products",
          text: "Comics",         
        },
        {
          href: "#about",
          text: "Movies", 
        },
        {
          href: "#contacts",
          text: "Tv",          
        },
        {
          href: "#blog",
          text: "Games",    
        },
        {
          href: "#blog",
          text: "Collectibles",    
        },
        {
          href: "#blog",
          text: "Videos",    
        },
        {
          href: "#blog",
          text: "Fans",    
        },
        {
          href: "#blog",
          text: "News",    
        },
        {
          href: "#blog",
          text: "Shop",    
        },
      ],
    };
  }
}

</script>


<template>
    <div class="d-flex" id="headerbox">
        <div class="d-flex" id="header">
            <div id="logoheader">
                <img src="../../img/dc-logo.png" alt="">
            </div>
            <div  id="nav" class="d-flex">
                <ul>
                    <li v-for="navitem in navData">{{navitem.text}}</li>
                </ul>
            </div>
        </div>
    </div>
</template>



<style scoped> 

#headerbox{
    justify-content: center;
    width: 100%;
}

#header{
    flex-direction: row;
    width: 80%;
    background-color: bisque; /*Debug feature*/ 

}

#logoheader{
    width: 20%;
}
#nav{
    width: 80%;
    justify-content: end;
}
li {
    font-weight: 500;
    padding: 0rem 1.25rem;
    margin-top: 40px;
}

li:hover{
    color: blue;
    border-bottom: solid blue;
}

ul{
    display: flex;
    text-align: center;
    list-style: none;
}

</style>