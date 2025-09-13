<script setup>
import { ref } from 'vue'

const msg = ref('Hello World!')
const header = ref('Shoping list')
const products = ref([{id:1,label:"product1"},{id:2, label:"product2"},{id:3,label: "product3"}])
</script>

<template>
  <h1>{{ msg }}</h1>
  <h2>{{header}}</h2>
<ul>
  <li v-for="product in products" :key="product.id">{{product.label}}</li>
</ul>
  <input v-model="msg" />
</template>
