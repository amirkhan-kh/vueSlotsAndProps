<template>
  <CardWrapper>
    <Container>
     <Card v-for="el in data" :key="el" :user="el"/>
    </Container>
  </CardWrapper>
  <MainLayout>
    <template #header="props">
      <header>
        <h1>{{ props.title }}</h1>
      </header>
    </template>

    <template #main="props">
        <main>
          <h1>{{ props.title }}</h1>
        </main>
    </template>

    <template #footer="props">
        <footer>
          <h1>{{ props.title }}</h1>
        </footer>
    </template>
  </MainLayout>

</template>

<script setup>
import Card from './components/card/index.vue'
import CardWrapper from './components/layout/card-wrapper/index.vue';
import Container from './components/layout/container/index.vue';
import MainLayout from './components/layout/main-layout.vue';
import {data} from './components/constants/index.js' 
</script>

<style lang="css" scoped>


</style>