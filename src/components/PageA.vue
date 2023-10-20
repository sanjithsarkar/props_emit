<script setup>
import PageB from './PageB.vue';
import { ref } from "vue";

const a = ref({
  a: 'a',
  b: 'b',
  c: 'c',
});

const eventData = ref('');

const handleEvent = (data) => {
  eventData.value = data;
};
</script>

<template>
  <PageB :testProps="a" @custom-event="handleEvent"></PageB>
  {{ eventData }}
</template>
