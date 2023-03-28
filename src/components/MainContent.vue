<script>
import { propsToAttrMap } from '@vue/shared';
import { onMounted } from 'vue';

    export default{
     name: 'MainContent', 
     props:{
            data: Array
        },
};


    
  
</script>

<template>
    <div id="maincontainer">
            <div id="adjustcontainer">
                <div id="subcontainer">
                    <div v-for="(card) in data" class="card">
                        <img :src="card.thumb" alt="">
                        <h4>{{card.series}}</h4>
                    </div>
                </div> 
            </div>
            <div id="bottomcontainer">
                <h3>LOAD MORE</h3>
            </div>
        </div>
        
</template>

<style scoped>

#maincontainer{
    background-color: black;
    display: flex;
    flex-direction: column;
    height: 600px;
}
#adjustcontainer{
    display: flex;
    flex-direction: row;
    justify-content: center;
    width: 100%;
}
#subcontainer{
    padding: 20px;
    width: 80%;
    height: 500px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
h4{
    color: white;
}

h3{
    display: inline;
    padding: 10px 40px;
    background-color: rgb(8, 103, 197);
    color: white;
}
#bottomcontainer{
    text-align: center;
}
.card{
    display: inline;
    text-align: center;
    height: 150px;
    width: calc(100% / 6);
}
.card img{
    height: 175px;
}

</style>