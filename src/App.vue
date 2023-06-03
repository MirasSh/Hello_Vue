<script setup>
import { ref } from 'vue'
import AboutView from '../src/views/AboutView.vue'

const products = ref([
  'Hello Vue',
  'Бананы',
  'Яблоки',
  'Груша',
  'Алма',
  'Нан',
  'Сүт',
  'Қызанақ',

])

</script>
<template>
  <div>
    <ul>
      <AboutView />
      <li v-for="product in products"
      :key="product"
      >
        {{ product }}
      </li>
    </ul>
  </div>
</template>

