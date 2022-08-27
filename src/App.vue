<template> 
    <h1 ref="agreet">Hello</h1>
    <input type="text" ref="name">
      <button @click="ClickMe">ClickMe</button>
      <!-- data go through parent to child -->
    <Modal :header="header" :content="content" :theme="theme" />
</template>

<script>
import Modal from "./components/Modal.vue";
export default {
  data(){
    return{
      // data binding
      header:"Login Success",
      content:"Welcome to Phyo Zay Yyar",
      theme:"success"
    }
  },
  methods:{
    ClickMe(){
      this.$refs.name.focus()
      this.$refs.agreet.textContent="Hee Hee"
    }
  },
  components:{
    Modal
  }
}
</script>

<style scoped>
/* css scoped */
  h1{
    color: blue;
  }
</style>