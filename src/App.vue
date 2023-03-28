<script>
import TheFooter from './components/TheFooter.vue';
import TheHeader from './components/TheHeader.vue';
import MainContent from './components/MainContent.vue';
import BottomBar from './components/BottomBar.vue';
import BlueBar from './components/BlueBar.vue';
import Data from './dc-comics.json'

export default {
      components:{
        TheFooter,
        TheHeader,
        MainContent,
        BottomBar,
        BlueBar,
    },
    data() {
      return{
        dataBase: Data,
      }
    }
  }
</script>

<template>
  <TheHeader></TheHeader>
  <MainContent :data="dataBase" ></MainContent>
  <BlueBar></BlueBar>
  <TheFooter></TheFooter>
  <BottomBar></BottomBar>
</template>

<style>

</style>
