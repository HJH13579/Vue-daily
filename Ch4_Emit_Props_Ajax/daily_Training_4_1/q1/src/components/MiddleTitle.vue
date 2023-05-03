<template>
  <div class="container">
    <div class="box">
      <div class="middle-title">
        <h2>{{ msg }}</h2>
      </div>
      
      <SmallTitle 
      :msg="smalltitlecontent"
      />
    </div>
  </div>
</template>

<script>
import SmallTitle from './SmallTitle.vue'

export default {
  name: 'MiddleTitle',
  props: {
    msg: String
  },
  components: {
    SmallTitle,

  },
  data() {
    return {
      smalltitlecontent: '시간선택',
    }
  },
}

</script>


<style scoped>
.container {
  display: flex;
  justify-content: center;
}

.box {
  width: 600px;
  height: 500px;
  background-color: #fff;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
}
</style>
