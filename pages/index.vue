<template>
  <div class="home-page">
   <div class="main-form">
     <div>{{count}}</div>
     <a-button style="border-radius: 0%; border: solid gray 1px">POP</a-button>
   </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { Button, message } from 'ant-design-vue';


export default Vue.extend({
  name: 'HomePage',
  components: {
    AButton: Button,
  },
  data() {
    return {
      count: 5000
    }

  }
  }
)
</script>

<style>
  .home-page {
    display: flex;
    justify-content: center;
    padding: 30px;
    }
  .main-form {
    background-color: #f2f3f4 ;
    padding: 30px;
    max-width: 400px;
    border: solid black 2px;
    }
  .count {
    color: brown;
    }
</style>
