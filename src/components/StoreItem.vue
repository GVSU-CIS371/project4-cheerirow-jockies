<template>
  <v-card class="ma-2 pa-2"
  :title="`${name}`"
  :text="`${description}`">
    <span>Rating: {{ rating }} <br> </span>
    <span>Price: {{ price  }} <br> </span>
    <span>Stock: {{ stock  }} <br> </span>
    <img :src="`${image}`" :height=150 :width=150>
  </v-card>
</template>

<script lang="ts" setup>
import { Product } from '../types/product';
defineProps<Product>();
</script>