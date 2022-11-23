<template lang="">
    <div class="componentside">

  <div class="top_side_left">
    <h5>Time Off</h5>
<div class="onsite">
<p>On-site</p>
<img src="../../assets/onsite.gif"/>
</div>
<div class="leave">
<p>Annual leave</p>
<h1>0.00</h1>
<p>Available days</p>
</div>
<div class="btns">
<button class="book">Book leave</button>
<button>My leave</button>
</div>
  </div>
  <div class="bottom_side_left">
    <div class="top_left"  >
<h4>Requests</h4>

    </div>

    <div class="bottom_left"  >
<div class="request">
    <p>Leave Request</p>
<img src="../../assets/chevon.png">
</div>
<div class="request">
    <p>Leave Request</p>
    <img src="../../assets/chevon.png">
</div>
<div class="request">
    <p>Procurement </p>
    <img src="../../assets/chevon.png">
</div>        
</div>
    </div>
    </div>
</template>
<script>


export default {
  name:"LeftView",

  
}
</script>
<style scoped>
  .onsite{
display: flex;
background-color: rgb(236, 56, 24);
 padding: 10px; 

 border-radius: 10px;
margin: 10px;
}  
  .onsite>img{
width: 100px;
height: 40px;
margin: 10px;
margin-left: 50px;

  }
  .onsite>p{
background-color: white;
border-radius: 50px;
color: #333;
padding: 3px;
font-size: 13px;
margin: 3px;
position: absolute;
margin-top: -8px;
  }
  .leave{
display: flex;
align-items: center;
justify-content: center;
flex-direction: column;
background-color: lightgray;
border-radius: 10px;
height: 140px;
font-size: 18px;
color: rgba(51, 51, 51, 0.89);
  }
  .leave>p{
      margin-bottom: -20px;
  }
  .leave>h1{
      margin-bottom: -20px;
  }
  .top_side_left{
background-color: white;
border-radius: 10px;

  }
  .top_side_left>h5{
font-size: 18px;
color: rgba(51, 51, 51, 0.527);
margin: 10px;

  }
  .btns{
      display: flex;
      align-items: center;
      justify-content:space-between;
      margin: 10px;
  }
  .btns>button{
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 10px;
      border: 1px solid orange;
      padding: 5px;
      border-radius: 8px;
  }
  .book{
background-color: orangered;
color: white;
  }
  .request{
display: flex;
align-items: center;
margin-left: 10px;
margin-bottom: -20px;
  }
  .top_left>h4{
    display: flex;
    border-bottom: 2px solid orangered;
align-items: center;
justify-content: center;
color: rgba(51, 51, 51, 0.801);
padding: 10px;
  }
  .bottom_side_left{
background-color: white;
border-radius: 10px;


  }
  .request>img{
width: 10px;
height: 10px;

  }
  .sidecomponent{
height: 100vh;
background-color: white;
  }
</style>