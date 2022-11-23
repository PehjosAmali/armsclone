<template >
    <div class="appbar">
      <div>

      </div>
      <div class="user_avatar">
          <div @click="show=true"  class="user">
          <p>Pehjos</p>
         <img src="../assets/avatar.png" />
      </div>  
      <div v-show="show" @click="show=false" class="showprofile">
<div class="list">
<img src="../assets/avatar.png"/>
<h4>Digital Profile</h4>
</div>
<div class="list">
<img src="../assets/ticket.png"/>
<h4>My Ticket</h4>
</div>
<div class="list">
<img src="../assets/lock.png"/>
<h4>Change</h4>
</div>
<div class="list">
<img src="../assets/switch.png"/>
<h4>Logout</h4>
</div>
    </div>
    </div>
 
    </div>
</template>
<script>
export default {
  name:"AppBar"  ,
  data() {
    return {
      show:false,
    }
}
}
</script>
<style scoped>
  .appbar{
display: flex;  
 justify-content: space-between;
 background-color: orange;   
 height: 60px;
width: 100%;
  }
  .user_avatar{
display: flex;
align-items: center;
background-color: rgb(240, 187, 89);
border-bottom-left-radius: 50px;
width: 200px;
justify-content:center;
  }
  .user{
    display: flex;
align-items: center;
background-color:white;
padding: 5px;
border-radius: 30px;
height: 30px;
  }
  .user>img{
      height: 30px;
      width: 30px;
  }

  .showprofile{
position: absolute;
margin-top: 260px;
background-color: white;
height: 200px;
border-radius: 10px;
width: 160px;
box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
  }
  .list{
display: flex;
align-items: center;
padding: 5px;
height: 30px;
/* margin: 10px; */
  }
  .list>img{
width: 20px;
border-radius: 50%;
height: 20px;
padding: 3px;
  }
  .list>h4{
font-size: 15px;
color: rgba(51, 51, 51, 0.658);

  }
  .list:hover{
background-color: orangered;

  }
</style>