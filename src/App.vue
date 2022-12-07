<script setup lang="ts">
import {useMainStore} from "./store/useMain"
import { storeToRefs } from 'pinia'

const main = useMainStore();

const{counter, name} = storeToRefs(main);
</script>

<template>

  <h3>hello world</h3>
  <h4>{{counter}}</h4>
</template>