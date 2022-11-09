<script setup lang="ts">
import dayjs from 'dayjs';

defineProps({
  title: {
    type: String,
    required: true,
  },
  start: {
    type: dayjs,
    required: true,
  },
  end: {
    type: dayjs,
    required: true,
  },
});

const array = new Array(9);
</script>

<template>
  <tbody>
    <tr>
      <th>一斉変更①</th>
      <td v-for="_ in array"></td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <th>一斉変更②</th>
      <td v-for="_ in array"></td>
    </tr>
  </tbody>
</template>
