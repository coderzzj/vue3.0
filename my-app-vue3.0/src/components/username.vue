<template>
  <div class="userName">
    <!-- 双向绑定v-modv-model用法 -->
    <input
      type="text"
      :value="title"
      @input="$emit('update:title', $event.target.value)"
    />
    userName:{{ title }}
    <!-- 多个v-model双向绑定 -->
    <input
      type="text"
      :value="firstName"
      @input="$emit('update:firstName', $event.target.value)"
    />
    <input
      type="text"
      :value="lastName"
      @input="$emit('update:lastName', $event.target.value)"
    />
  </div>
</template>

<script>
export default {
  data () {
    return {

    }
  },
  props: {
    title: {
      type: String,
    },
    firstName: {
      type: String
    },
    lastName: {
      type: String
    }
  },
  emits: ["update:title", "update:firstName", "update:lastName"]
}
</script>

<style>
</style>