<template lang="">
    <div class="dirHead">
   <h5>Home</h5>/
   <p>Directory</p>
    </div>
</template>
<script>
export default {
  name:"DirectoryHead"  
}
</script>
<style scoped>
  .dirHead{
display:flex ;
margin: 20px;
padding: 3px;
height: 40px;
background-color: white;
box-shadow: rgba(0, 0, 0, 0.08) 0px 4px 12px;
align-items: center;
  }  
  
  .dirHead>h5{
color: orangered;

font-size: 14px;
  } 
  .dirHead>p{
color: rgba(51, 51, 51, 0.705);

font-size: 13px;
  }
</style>