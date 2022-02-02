<template>
  <div class="hero">
    <div class="name"> 
    Hello! <br>
     I am Ntombizanele<br>
     an aspiring Software Developer
    </div>
  </div>
</template>

<script>
export default {
name:"hero",
components:{
},
data() {
    return {
        
    }
},
}
</script>

<style scoped>
.hero{
    background: linear-gradient(135deg, #e55d87 0%, #5fc3e4 100%);
    height: 300px;
    text-align: center;
    padding-bottom: 71px;
    margin-left: 180px;
}
.name{
  padding: 71px;
  font-size: 50px;
  text-align: left;
  font-family: normal;
}
</style>