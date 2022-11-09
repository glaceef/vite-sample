<script setup lang="ts">
import dayjs from 'dayjs';
import ScheduleGanttChartDateRangeRow from '../components/ScheduleGanttChartDateRangeRow.vue';
import ScheduleGanttChart from '../components/ScheduleGanttChart.vue';

const start = dayjs();
const end = start.add(2, 'w');
</script>

<template>
  <ScheduleGanttChart :start="start" :end="end">
    <ScheduleGanttChartDateRangeRow
      title="タイトル"
      :start="start"
      :end="end"
    />
  </ScheduleGanttChart>
</template>
