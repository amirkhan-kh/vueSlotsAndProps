<template>
     <div class="card">
        <img src="https://picsum.photos/id//450/150/200/" alt="">
        <div class="card-body">
          <h5 class="card-title">Card title</h5>
          <p class="card-text">{{ user.name }}</p>
          <p>age {{ user.age }}</p>
          <button @click="messageDelete">show</button>
        </div>
      </div>
</template>
<script setup>
import { defineProps, ref } from 'vue';
const prop = defineProps({
  user:{
    type:Object,
    required:true,
    default:()=>({name:'John Doe', age:30}) 
  }
})
const messageDelete = () => {
  alert(prop.user.name)
}
</script>
<style src="./style.css" scoped></style>