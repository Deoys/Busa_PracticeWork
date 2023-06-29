<template>
    <Chart
      :options="{
    width: '100%',
    symbol: 'BITSTAMP:BTCUSD',
    interval: D,
    timezone: Etc/UTC,
    theme: light,
    style: 1,
    locale: ru,
    toolbar_bg: '#F3F9FF',
    backgroundColor: '#F3F9FF',
    enable_publishing: false,
    hide_top_toolbar: true,
    hide_legend: true,
    save_image: false,
      }"
    />
  </template>
  
  <script>
  import { Chart } from "vue-tradingview-widgets";
  
  export default {
    name: "chartContainer",
    components: {
      Chart,
    },
  };
  </script>