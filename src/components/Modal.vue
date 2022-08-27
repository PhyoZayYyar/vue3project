<template>
  <div class="drop">
    <div class="modal">
      <h1>Modal</h1>
        <p>This Modal Content Box</p>
    </div>
  </div>
</template>

<script>
export default {

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
</style>