<template>
  <header>
    <h1>{{ propsdata }}</h1>
    <button v-on:click="sendEvent">send</button>
  </header>
</template>

<script>
export default {
  props: ['propsdata'],
  methods: {
    sendEvent() {
      this.$emit('renew');
    }
  }
}
</script>

<style>

</style>