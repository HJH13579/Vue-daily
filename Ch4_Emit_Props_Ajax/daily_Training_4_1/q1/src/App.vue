<template>
  <div id="app">
    <BigTitle 
      :msg="bigtitlecontent"
    />
    <MiddleTitle 
      :msg="middletitlecontent"
    />
  </div>
</template>

<script>
import BigTitle from './components/BigTitle.vue'
import MiddleTitle from './components/MiddleTitle.vue'

export default {
  name: 'App',
  components: {
    BigTitle,
    MiddleTitle,
  },
  data() {
    return {
      bigtitlecontent: '버튼 박스 제작',
      middletitlecontent: '예약 페이지',
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
