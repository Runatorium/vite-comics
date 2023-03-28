<script>
import { propsToAttrMap } from '@vue/shared';
import { onMounted } from 'vue';

    export default{
     name: 'MainContent', 
     props:{
            data: Array
        },
        setup(props){
        onMounted(()=>{
            console.log(props.data)
        });    
    },
};


    
  
</script>

<template>
    <div id="maincontainer">
        <div id="subcontainer">
            <div v-for="(card) in data" class="card">
                <img :src="card.thumb" alt="">
                <h4>{{card.series}}</h4>
            </div>
        </div>
    </div>

</template>

<style scoped>

#maincontainer{
    background-color: black;
    display: flex;
    justify-content: center;
    widows: 100%;
    height: 500px;
}

#subcontainer{
    padding: 20px;
    width: 80%;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
h4{
    color: white;
}
.card{
    text-align: center;
    height: 150px;
    width: calc(100% / 6);
}
.card img{
    height: 150px;
    widows: 150px;
}

</style>