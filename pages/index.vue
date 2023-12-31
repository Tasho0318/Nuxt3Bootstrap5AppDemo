<template>
    <div>
      <h1>Red Bull サイト</h1>
      <div v-if="redbullInfo">
        <h2>{{ redbullInfo.name }}</h2>
        <p>{{ redbullInfo.description }}</p>
        <img :src="redbullInfo.image" alt="Red Bull">
      </div>
      <div v-else>
        <p>データを取得中...</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    async asyncData({ $axios }) {
      try {
        const response = await $axios.get('https://api.example.com/redbull'); // Red BullのAPIエンドポイントを実際のものに変更してください
        return { redbullInfo: response.data };
      } catch (error) {
        console.error('APIエラー:', error);
        return { redbullInfo: null };
      }
    },
  };
  </script>
  