<template lang="">
    <div class="home_components">
        <div class="left">
      <LeftView/>
    </div>
    <div class="middle">
      <MiddleView
      price1="₵120,0000"
      price2="₵60,0000"
      price3="₵2,0000"
      />
      </div>
      <div class="right">
      <RightView/>  
    </div>
    </div>
</template>
<script>
import LeftView from './LeftView.vue';
import RightView from './RightView.vue';
import MiddleView from './MiddleView.vue'

export default {
components:{
    LeftView,
    RightView,
    MiddleView,
},

    name:"HomeView" 
}
</script>
<style scoped>
  .home_components{
display: flex;
align-items: center;
justify-content: space-between;
/* margin: 10px; */
  }  
  .left{

    display: flex;
align-items: center;
justify-content: space-between; 
flex-direction: column;
height: 100vh;
flex: 0.2;
  }
  .middle{

display: flex;
align-items: center;
justify-content: space-between; 
flex-direction: column;
height: 100vh;
flex: 0.6;
}
.right{

display: flex;
align-items: center;
justify-content: space-between; 
flex-direction: column;
height: 100vh;
flex: 0.2;
}
</style>