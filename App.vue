<template>
  <!-- <HelloWorld />
         <IfDemo/>
         <ListDemo/>
         <KeyDemo/>
         <EventDemo1/> 
         <EventDemo2/> 
         <EventDemo3/>
         <EventDemo4/> -->
         <!-- <Header/>
         <Main/>
         <Aside/> 
         <Parent/>-->
         <!--<ComponentA/>
          <ComponentEvent/>
         <Main/> -->
  <!-- <SlotsBase>
    <div>
      <h3>插槽标题</h3>
      <p>插槽内容</p>
    </div>
  </SlotsBase> -->
  <!-- <SlotsTwo>
    <template #header >
      <h3>{{ message }}</h3>
    </template>
    <template #smain >
     <p>内容</p>
    </template>
  </SlotsTwo> -->
  <SlotsAttr >
    <template #header="slotProps">
      <h3>{{ currentTest }}-{{ slotProps.msg }}</h3>
    </template>
    <template #main="slotProps">
      <P>{{ slotProps }}</P>
    </template>
  </SlotsAttr>
</template>
<!-- <script setup>
import HelloWorld from './components/HelloWorld.vue'
import IfDemo from './components/IfDemo.vue'
import ListDemo from './components/ListDemo.vue'
import KeyDemo from './components/KeyDemo.vue'
import EventDemo1 from './components/EventDemo1.vue'
import EventDemo2 from './components/EventDemo2.vue'
import EventDemo3 from './components/EventDemo3.vue'
import EventDemo4 from './components/EventDemo4.vue'
import ClassDemo from './components/ClassDemo.vue'
import StyleDemo from './components/StyleDemo.vue'
import WatchDemo from './components/WatchDemo.vue'
</script> -->
<script>
//import Header from './pages/Header.vue'
// import Main from './pages/Main.vue'
// import Aside from './pages/Aside.vue'
// import Parent from './components/Parent.vue'
/* import ComponentA from './components/ComponentA.vue'
import ComponentEvent from './components/ComponentEvent.vue'
import Main from './components/Main.vue' */
import SlotsBase from './components/SlotsBase.vue'
import SlotsTwo from './components/SlotsTwo.vue'
import SlotsAttr from './components/SlotsAttr.vue'

export default {
  data(){
    return{
      message:"插槽内容续集",
      currentTest:"测试内容"
    }
  },
  components:{
    //   Parent
    //Header,
   // Main,
    //Aside
    /* ComponentEvent,
    Main, */
    //ComponentA
    SlotsBase,
    SlotsTwo,
    SlotsAttr
  }
  
}
</script>
