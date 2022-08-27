<template>
  <div class="drop">
    <div class="modal" :class="{success:theme==='success', danger:theme==='danger'}">
      <h1>{{header}}</h1>
      <p>{{content}}</p>
    </div>
  </div>
</template>

<script>
export default {
  props:["header","content","theme"]
}
</script>

<style scoped>
  .drop{
    position: fixed;
    top:0;
    width:100%;
    height:100%;
    background-color: rgba(0, 0, 0, 0.5);
  }
  .modal{
    width: 400px;
    margin:100px auto;
    padding:20px;
    background-color: aliceblue;
    border-radius: 10px;
  }
  p{
    font-style: normal;
  }
  .success{
    background-color: green;
    color:white;
  }
  .danger{
    background-color:rgb(199, 84, 84);
    color:white;
  }
</style>