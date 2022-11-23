<template lang="">
    <div class="filters">
       <div class="dir">
<p>Directory</p>
       </div> 
       <div class="inputs">
           <div class="search">
               <input type="text" placeholder="search..."/>
               <img src="../../assets/search.png"/>
           </div>
        <select>
<option>Department</option>
        </select>   
        <select>
<option>userType</option>
        </select> 
        <select>
<option>status</option>
        </select> 
        <button class="btn">Filter</button>   
        <button>Reset</button> 
        </div>
    </div>
</template>
<script>
export default {
 name:"FilterSearch", 
}
</script>
<style scoped>
    .inputs{
display: flex;
align-items: center;
justify-content: space-between;
margin: 20px;
    }

.search{
  display: flex; 
  align-items: center; 
  padding: 3px;
  border-radius: 10px;
  border: 1px solid lightgrey;
  background-color: white;
  width: 230px;
}
.search>input{
  border: none;
  outline-width: 0;

}
.inputs>select{
width: 200px;
height: 40px;
border: 1px solid lightgray;
border-radius: 10px;
color: rgba(51, 51, 51, 0.548);
outline-width: 0;
font-weight: bold;
font-size: 17px;
}
.inputs>button{
width: 100px;
height: 30px;
border: 1px solid orange;
border-radius: 10px;
color: orange;
outline-width: 0;
font-weight: bold;
font-size: 15px;
}
.btn{
background-color: orangered;
color: white !important;
}
.dir{
margin: 20px;

}
.dir>p{
font-weight: bold;
color: gray;

}
</style>