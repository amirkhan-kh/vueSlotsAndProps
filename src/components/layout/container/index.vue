<template>
    <div class="container">
        <slot/>
    </div>
</template>

<script setup>

</script>

<style  scoped>
.container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 30px 20px;
}
</style>