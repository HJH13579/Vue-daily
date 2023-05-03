<template>
  <div class="small-title">
    <h3>{{ msg }}</h3>
    <div class="button-box" v-for="(time, index) in times" :key="index">{{ time }}</div>

  </div>
</template>

<script>
export default {
  name: 'SmallTitle',
  props: {
    msg: String
  },
  data () {
    return {
      times: [
        "09:00","09:30","10:00","10:30","11:00","11:30","12:00","12:30","13:00","13:30",
        "14:00","14:30","15:00","15:30","16:00","16:30","17:00","17:30","18:00","18:30",
        "19:00","19:30","20:00","20:30","21:00","21:30","22:00","22:30","23:00","23:30",
      ]
    }
  }
}
</script>


<style scoped>
.button-box {
  width: 100px;
  height: 100px;
  background-color: #fff;
}

</style>
