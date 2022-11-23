<template lang="">
    <div class="staffCard">
      <div class="img_name" >
<img :src="image" alt/>
<h5>{{name}}</h5>
      </div> 
     <div class="menu_toggle" >
      <img @mouseover="showphone=true" @mouseleave="showphone=false" src="../../assets/phone.png" alt=""/>   
      <img @mouseover="showemail=true" @mouseleave="showemail=false" src="../../assets/envolope.png" alt=""/>  
      <img src="../../assets/person.png" alt=""/>  
     </div>
     <div class="display">
<p v-show="showphone">{{phone}}</p>
<p v-show="showemail">{{email}}</p>
<p>{{position}}</p>
     </div>
<div class="personettpe">
<p>{{jobtype}}</p>
<p>{{location}}</p>

</div>

    </div>
</template>
<script>


export default {
   name:"StaffCard" ,
   props:{
image:String,
phone:String,
location:String,
jobtype:String,
name:String,
email:String,
position:String,

   },
   data(){
return{
showphone:false,
showemail:false
}

   }
}
</script>
<style scoped>
 .img_name>img{
width: 100px;
border-radius: 50%;
height: 100px;
 } 
 .staffCard{
display: flex;
align-items: center;
justify-content: center;
margin: 10px;
height: 350px;
border-radius: 10px;
background-color: white;
width: 280px;
flex-direction: column;
 } 
 .img_name{
display: flex;
align-items: center;
justify-content: center;
flex-direction: column;
 } 
 .menu_toggle{
display: flex;
align-items: center;

justify-content: space-between;
 }
 .menu_toggle>img{
width: 15px;
height: 15px;
margin: 20px;
    display: flex;
align-items: center;
justify-content: space-between; 
 }
 .display>p{
     background-color: pink;
position: absolute;
border-top-left-radius: 10px;
border-top-right-radius: 10px;
padding: 3px;
margin: 10px;
display: flex;
align-items: center;
justify-content: center;
margin-left: -70px;
margin-top: -10px;
 }
 .personettpe{
display: flex;
align-items: center;
justify-content: center;
flex-direction: column;
 }
 .personettpe>p{
display: flex;
align-items: center;
justify-content: center;
padding: 2px;
margin-bottom: -10px;
height: 20px;
width: 200px;
border: 1px solid lightgrey;
border-radius: 30px;
flex-direction: column;
 }
</style>