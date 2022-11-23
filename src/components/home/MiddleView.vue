<template >
    <div class="main">
    <div class="apps">
   <p>Apps</p>  
   
   <div class="apps_list">
<div class="single_App" @mouseover="show=true" @mouseleave="show=false">
    <p>Assesment</p>
    <img src="../../assets/assesment.png"/>
    <div v-show="show"  class="hover">
<p>self assesment</p>
<p>Peer review</p>
    </div>
</div>
<div class="single_App" @mouseover="showDir=true" @mouseleave="showDir=false">
    <p>Directory</p>
    <img src="../../assets/contact.png"/>

    <div v-show="showDir" class="staff">
        <a href="#/staff">All Staff</a> 
    </div>
</div>
<div class="single_App">
    <p>Finance</p>
    <img src="../../assets/bookmark.png"/>
</div>
<div class="single_App">
    <p>Loans</p>
    <img src="../../assets/file.png"/>
</div>
<div class="single_App">
    <p>Pols . & Docs</p>
    <img src="../../assets/doc.png"/>
</div>
<div class="single_App">
    <p>Procurement</p>
    <img src="../../assets/cart.png"/>
</div>
   </div>

    </div>

    <div class="numeric">
    <div class="numeric1">

<h3>{{price1}}</h3>
    
</div>
<div class="numeric2">
    <h3>{{price2}}</h3>

    
</div>
<div class="numeric3">

    <h3>{{price3}}</h3>
    
</div>
</div>
<div class="anouncement">
<p>Announcement</p>
<div class="anouncements">

<p>No New Notification</p>
<img src="../../assets/waves.png"/>
</div>
</div>
</div>

</template>
<script>
export default {
    name:"MiddleView",
   props:{
price1:String,
price2:String,
price3:String,
   },
   data() {
       return {
         show:false,  
         showDir:false,
       
       }
   },
  
}
</script>
<style scoped>
    .apps_list{
display: flex;
align-items: center;
justify-content: space-between;
margin-left: 50px;
    }
    .single_App{
display: flex;
margin: 10px;
flex-direction: row-reverse;
margin-top: -6px;
    }
    .single_App>img{
width: 20px;
height: 20px;
color: red;
border-radius: 50%;
padding: 5px;
background-color: rgb(255, 205, 192);
    }
    .apps{
background-color: white;
height: 100px;
border-radius: 10px;
box-shadow: rgba(0, 0, 0, 0.08) 0px 4px 12px;
    }
    .apps>p{
margin: 10px;

    }
    .numeric{
display: flex;
align-items: center;
justify-content: space-between;
margin-top: 10px;
color: white;
    }
    .numeric1{
display: flex;
align-items: center;
justify-content: center;
background-color: rgba(255, 123, 0, 0.842);
border-radius: 10px;
width: 230px;
height: 90px;

    }
    
    .numeric2{
display: flex;
align-items: center;
justify-content: center;
background-color:rgb(160, 148, 148);
border-radius: 10px;
width: 230px;
height: 90px;

    }
    
    .numeric3{
display: flex;
align-items: center;
justify-content: center;
background: rgb(219,71,16);
background: linear-gradient(90deg, rgba(219,71,16,0.5326505602240896) 97%, rgba(227,41,13,0.09567577030812324) 100%);
border-radius: 10px;
width: 230px;
height: 90px;

    }
    .anouncement{
width: 100%;
background-color: white;
height: 300px;
border-radius: 10px;

    }
.anouncement>p{
font-size: 18px;
font-weight: bolder;
margin: 10px;
color: rgba(51, 51, 51, 0.767);
}
    .anouncements{
height: 250px;
border-radius: 30px;
background-color: whitesmoke;
margin: 20px;
display: flex;
align-items: center;
font-size: 20px;
color: rgba(51, 51, 51, 0.514);
font-weight: bold;
align-content: center;
flex-direction: column;
    }
    .hover{
position: absolute;
margin-top: 30px;
width: 130px;
background-color: white;
border-radius: 10px;
padding: 10px;
height: 70px;
margin-left: 30px;
box-shadow: rgba(0, 0, 0, 0.08) 0px 4px 12px;
    }
    .hover>p:hover{
background-color: lightgray;
cursor: pointer;
    }
    .staff{
position: absolute;
margin-top: 30px;
text-align: center;
width: 130px;
height: 40px;
background-color: white;
box-shadow: rgba(0, 0, 0, 0.08) 0px 4px 12px;
border-radius: 10px;
    }
</style>