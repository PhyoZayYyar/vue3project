<template> 
    <h1 ref="agreet">Hello</h1>
    <input type="text" ref="name">
    <button @click="ClickMe">ClickMe</button>
    <Modal/>
</template>

<script>
import Modal from "./components/Modal.vue";
export default {
  data(){
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

<style>

</style>