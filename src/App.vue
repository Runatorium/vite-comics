<script>
import TheFooter from './components/TheFooter.vue';
import TheHeader from './components/TheHeader.vue';
import MainContent from './components/MainContent.vue';
import BottomBar from './components/BottomBar.vue';
import BlueBar from './components/BlueBar.vue';
import Data from './dc-comics.json'
import JumboTron from './components/JumboTron.vue'

export default {
      components:{
        TheFooter,
        TheHeader,
        MainContent,
        BottomBar,
        BlueBar,
        JumboTron,
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
  <JumboTron></JumboTron>
  <MainContent :data="dataBase" ></MainContent>
  <BlueBar></BlueBar>
  <TheFooter></TheFooter>
  <BottomBar></BottomBar>
</template>

<style>

</style>
