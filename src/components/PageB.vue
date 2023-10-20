<script setup>
import { ref, defineProps, defineEmits } from 'vue';

const props = defineProps(['testProps']);
const emit = defineEmits(['custom-event']);

const data = ref('emit testing');

const emitEvent = () => {
  emit('custom-event', data);
};
</script>

<template>
  <span v-for="(test, index) of props.testProps">{{ test }}</span>

  <button @click="emitEvent">Emit Event</button>
</template>
