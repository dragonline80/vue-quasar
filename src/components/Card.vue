<template lang="">
  <q-card>
    <div class="text-center bg-primary text-white">
      {{ members.title }}
    </div>
    <q-card-section>
      <div>{{ members.name }}</div>
      <div>{{ members.part }}</div>
      <div>{{ members.tel }}</div>
    </q-card-section>
  </q-card>
</template>
<script setup>
import { ref, defineProps } from 'vue'

const props = defineProps({
  members: {
    type: Array
  }
})
const cardList = ref()
</script>
<style lang="sass" scoped></style>
