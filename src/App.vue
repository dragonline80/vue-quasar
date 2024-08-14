<script setup>
import Card from './components/Card.vue'
import memberData from './assets/data/member'
import { ref } from 'vue'

const members = ref(memberData)
</script>

<template>
  <div class="row q-gutter-lg">
    <Card v-for="(item, index) in members" :key="index" :members="item"></Card>
  </div>
</template>

<style scoped></style>
