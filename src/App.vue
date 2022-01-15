<template>
<body>
   <!-- <div> -->
    <!-- primary button -->
    <!-- <div>
      <primaryButton value="Click here"></primaryButton>
      <br>
      <primaryButton value=" or Click here"></primaryButton>
    </div> -->
    <!-- data return -->
    <!-- <div>
       <dataReturn value="cup of tea"></dataReturn>
    </div>   -->
  <!-- </div> -->
  <!-- attribute bind -->
  <!-- <div>
      <attributeBind></attributeBind>
  </div> -->
  <!-- conditional render -->
  <!-- <div>
      <conditionalRender></conditionalRender>
  </div> -->
  <!-- list render -->
  <!-- <listRender></listRender> -->
    <!-- Event handel -->
    <!-- <EventHandel></EventHandel> -->
    <classStyleBind></classStyleBind>
 
</body>
 


</template>
<script>
  // import primaryButton from './components/primaryButton.vue'
  // import dataReturn from './components/dataReturn.vue'
  // import attributeBind from './components/attributeBind.vue'
  // import conditionalRender from './components/conditionalRender.vue'
  // import listRender from './components/listRender.vue'
  // import EventHandel from './components/EventHandel.vue'
  import classStyleBind from './components/classStyleBind.vue'
 
  export default {
    name: 'app',
    components: {
      // primaryButton,
      // dataReturn,
      // attributeBind,
      // conditionalRender,
        // listRender,
        // EventHandel,
        classStyleBind       
    }
  }
</script>

<style>
     body {
  background-color: #f2f2f2;
  margin: 0px;
  font-family: tahoma;
  color: #282828;
}
img {
  border: 2px solid #d8d8d8;
  width: 20%;
  height: 20%;
  margin: 40px;
  padding: 15px;
  -webkit-box-shadow: 0px 2px 15px -12px rgba(0, 0, 0, 0.57);
  -moz-box-shadow: 0px 2px 15px -12px rgba(0, 0, 0, 0.57);
  box-shadow: 2px 15px -12px rgba(0, 0, 0, 0.57);
}
.disabledButton {
  background-color: #d8d8d8;
  cursor: not-allowed;
}
.out-of-stock-img {
  opacity: 0.5;
}




</style>


