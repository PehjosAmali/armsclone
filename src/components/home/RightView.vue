<template lang="">
    <div class="mainside">
    <div class="quaote">
      <h4>Quote of the day</h4>
      <p>Never let lack of money interfere with having fun.</p>
    </div>
    <div class="out">
<h4>Who is out</h4>
<p>Today(1)</p>
<img src="https://media-exp1.licdn.com/dms/image/C5603AQHXO62dyzbdTw/profile-displayphoto-shrink_200_200/0/1618510493844?e=1674691200&v=beta&t=LLgmd2Ip6gZ7DPxkdYAV75xeNB1Do4txEglSSPLaAcE"/>
<p>Tomorrow(1)</p>
<p>Next Week(17)</p>
<div class="outimg">
<img src="https://media-exp1.licdn.com/dms/image/C5603AQHXO62dyzbdTw/profile-displayphoto-shrink_200_200/0/1618510493844?e=1674691200&v=beta&t=LLgmd2Ip6gZ7DPxkdYAV75xeNB1Do4txEglSSPLaAcE"/>
<img src="https://media-exp1.licdn.com/dms/image/C5603AQHXO62dyzbdTw/profile-displayphoto-shrink_200_200/0/1618510493844?e=1674691200&v=beta&t=LLgmd2Ip6gZ7DPxkdYAV75xeNB1Do4txEglSSPLaAcE"/>
</div> 

</div>
<div class="celebration">
<h4>Celebration</h4>
<div class="people">
    <img src="https://media-exp1.licdn.com/dms/image/C5603AQHXO62dyzbdTw/profile-displayphoto-shrink_200_200/0/1618510493844?e=1674691200&v=beta&t=LLgmd2Ip6gZ7DPxkdYAV75xeNB1Do4txEglSSPLaAcE"/>
<div class="content_p">
 <h4>Charles Kwame Amo</h4>  
 <p>Nov 23 - Happy Birthday!</p> 
</div>
</div>
<div class="people">
    <img src="https://media-exp1.licdn.com/dms/image/C5603AQHXO62dyzbdTw/profile-displayphoto-shrink_200_200/0/1618510493844?e=1674691200&v=beta&t=LLgmd2Ip6gZ7DPxkdYAV75xeNB1Do4txEglSSPLaAcE"/>
<div class="content_p">
 <h4>Charles Kwame Amo</h4>  
 <p>Nov 23 - Happy Birthday!</p> 
</div>
</div>
</div>
</div>
</template>
<script>
export default {
    name:"RightView" 
}
</script>
<style scoped>
    .quaote{
background-color: white;
margin: 10px;
color: rgba(51, 51, 51, 0.781);
border-radius: 10px;
height: 90px;
    }
    .quaote>h4{
background-color: white;
margin: 16px;
    }
    .quaote>p{
background-color: white;
margin: 10px;

    }
   .out{
background-color: white;
border-radius: 10px;
height: 190px;
margin: 10px;
padding: 10px;
   } 
    .out>h4{
font-size: 13px;
color: rgba(51, 51, 51, 0.849);

    }
.out>p{
font-size: 12px;

}
    .out>img{
height: 30px;
width: 30px;
border-radius: 50%;

    }
    .outimg>img{
        height: 30px;
width: 30px;
border-radius: 50%;
margin-top: -10px;
    }
    .celebration{
background-color: white;
height: 180px;
margin: 10px;
border-radius: 10px;
    }
    .celebration>h4{
margin: 10px;
color: rgba(51, 51, 51, 0.76);
    }
    .people>img{
        height: 30px;
width: 30px;
border-radius: 50%;

    }
    .people{
display: flex;
align-items: center;
padding: 10px;
    }
    .content_p>h4{
color: rgba(51, 51, 51, 0.795);
font-size: 13px;
    }
    .content_p>p{
margin-bottom: -10px;
font-size: 10px;
    }
</style>