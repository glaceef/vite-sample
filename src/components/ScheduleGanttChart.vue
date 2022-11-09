<script setup lang="ts">
import dayjs from 'dayjs';

defineProps({
  start: {
    type: dayjs,
    required: true,
  },
  end: {
    type: dayjs,
    required: true,
  },
});
</script>

<template>
  <table border="1">
    <thead>
      <tr>
        <th />
        <th colspan="3">2000年 1月</th>
        <th colspan="3">2000年 2月</th>
        <th colspan="3">2000年 3月</th>
      </tr>
      <tr>
        <th />
        <th style="width: 24px">1</th>
        <th style="width: 24px">...</th>
        <th style="width: 24px">31</th>
        <th style="width: 24px">1</th>
        <th style="width: 24px">...</th>
        <th style="width: 24px">29</th>
        <th style="width: 24px">1</th>
        <th style="width: 24px">...</th>
        <th style="width: 24px">31</th>
      </tr>
    </thead>
    <slot />
  </table>
</template>
