<template>
  <div>
    <username v-model:msg="msg"></username>
    {{ msg }}
  </div>
</template>

<script>
import username from "./username.vue"
export default {
  data () {
    return {
      msg: "hello vue3.0"
    }
  },
  component: {
    username
  }
}
</script>

<style>
</style>