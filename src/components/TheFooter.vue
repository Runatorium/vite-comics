<script>

    export default{
        name: 'TheFooter',
        data() {
            return {
                dcComics:[
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                    "Games",
                    "Videos",
                    "News",
                 ],
                 Shop: [
                    "Shop Dc",
                    "Shop Dc Collectibles"
                 ],
                Dc: [
                    "Terms of Use",
                    "Privacy Policy (new)",
                    "Ad Choices",
                    "Advertising",
                    "Jobs",
                    "Subscription",
                    "Talents Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact Us",
                ],
                Sites: [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa",
                ]
    
            };
        },      
    }

</script>

<template>
    <footer class="d-flex">
        <div class="internalcontainer d-flex">
        <div id="leftcontainer">
            <div>
                <ul>
                    <li id="title">Dc Comics</li>
                    <li v-for="(data, i) in dcComics" :key="i" class="item">{{data}}</li>
                </ul>
                <ul>
                    <li id="title">Shop</li>
                    <li v-for="(data, i) in Shop" :key="i" class="item">{{data}}</li>
                </ul>
            </div>
            <div>
                <ul>
                    <li id="title">DC</li>
                    <li v-for="(data, i) in Dc" :key="i" class="item">{{data}}</li>
                </ul>
            </div>
            <div>
                <ul>
                    <li id="title">Sites</li>
                    <li v-for="(data, i) in Sites" :key="i" class="item">{{data}}</li>
                </ul>
            </div>
        </div>
        <div id="rightcontainer">
        </div>
        </div>
    </footer>

</template>

<style scoped>

footer{
    width: 100%;
    justify-content: center;
    background-image: url(../../img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 450px;
}  

.internalcontainer{
    justify-content: space-between;
    width: 80%;
}
.item{
    color: grey;
    padding: 2px;
    font-size: 12px;
}
ul{
    padding: 10px;
    list-style: none;
    color: white;
    margin-top: 20px;
}
#title{
    margin-bottom: 20px;
    font-size: 24px ;
}

#rightcontainer{
        width: 50%;
        background-position: 100%;
        background-repeat: no-repeat;
        background-image: url(../../img/dc-logo-bg.png);  
    }

#leftcontainer{
        display: flex;
        flex-direction: row;
    }
</style>