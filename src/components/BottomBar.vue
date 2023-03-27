<script>
 export default{
    name: 'BottomBar',
    data() {
            return {
                icons: [
                    {
                        name: "facebook",
                        icon: "fa-facebook"
                    }
                ]
             }
         }
 };
</script>

<template>
    <div class="bottombar">
        <div class="innerbox">
            <div>
                <h1>SIGN UP NOW</h1>
            </div>
            <div class="rightbox">
                <ul class="d-flex">
                    <h2>FOLLOW US</h2>
                    <ul id="iconlist" class="d-flex">
                        <li><i class="fa-brands fa-facebook"></i></li>
                        <li><i class="fa-brands fa-twitter"></i></li>
                        <li><i class="fa-brands fa-youtube"></i></li>
                        <li><i class="fa-brands fa-pinterest"></i></li>
                        <li><i class="fa-solid fa-location-dot"></i></li>
                    </ul>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>

.innerbox{
    width: 80%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
.bottombar{
    display: flex;
    justify-content: center;
    background-color: rgb(37, 37, 37);
    color: white;
    height: 150px;
}
.rightbox{
    display: flex;
    align-self: center;

}
ul{
    flex-direction: row;
    list-style: none;
    justify-content: space-between;
}
i{
    padding: 10px;
    color: grey;
    font-size: 36px;
}
h1{
    align-items: center;
    margin-top: 50px;
    font-size: 24px;
    display: inline-block;
    padding: 8px;
    border: solid 2px  rgb(72, 127, 215);
}
h2{
    align-self: center;
    color: rgb(72, 127, 215) ;
}
</style>