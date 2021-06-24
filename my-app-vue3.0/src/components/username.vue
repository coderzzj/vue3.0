<template>
  <div id="son">
    <input
      type="text"
      :value="msg"
      @input="$emit('update:msg', $event.target.value)"
    />
    {{ msg }}
  </div>
</template>

<script>
export default {
  data () {
    return {

    }
  },
  props: {
    msg: {
      type: String,
    }
  },
  emits: ["update:msg"]
}
</script>

<style>
</style>