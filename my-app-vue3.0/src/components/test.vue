<template>
  <div>
    <!-- 父组件 -->
    <user-name v-model:title="msg"></user-name>
    test:{{ msg }}

    <user-name
      v-model:firstName="firstName"
      v-model:lastName="lastName"
    ></user-name>
    {{ firstName }}---{{ lastName }}
  </div>
</template>

<script>
import UserName from "./username.vue"
export default {
  data () {
    return {
      msg: "hello vue3.0",
      firstName: "zhou",
      lastName: "ddddd"
    }
  },
  components: {
    UserName
  }
}
</script>

<style>
</style>