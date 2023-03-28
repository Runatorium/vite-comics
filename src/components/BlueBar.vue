<script>
export default{
    name: 'BlueBar',
    data() {
            return {
                blueImgs: [
                    {
                        img: '../../img/buy-comics-digital-comics.png',
                        text: 'Digital Comics'
                    },
                    {
                        img: '../../img/buy-comics-merchandise.png',
                        text: 'DC Merchandise'
                    },
                    {
                        img: '../../img/buy-comics-subscriptions.png',
                        text: 'Subscription'
                    },
                    {
                        img: '../../img/buy-comics-shop-locator.png',
                        text: 'Comic Shop Locator'
                    },
                    {
                        img: '../../img/buy-dc-power-visa.svg',
                        text: 'DC Power Visa'
                    }
                ]
             }
         }
 };
</script>

<template>
    <div class="bluebar">
        <div class="innerbox">
            <div class="box" v-for="(item, i) in blueImgs" :key="i">
                <img :src="item.img" alt="">
                <h4>{{item.text}}</h4>
            </div>
        </div>
    </div>  
</template>

<style scoped>

.bluebar{
    width: 100%;
    height: 150px;
    background-color: rgb(8, 103, 197);
    display: flex;
    justify-content: center;
}
.innerbox{
    widows: 80%;
    display: flex;
    justify-content: space-between;
}
.box{
    display: flex;
    align-items: center;
    color: white;
}

.box img{
    width: 50%;
}

</style>