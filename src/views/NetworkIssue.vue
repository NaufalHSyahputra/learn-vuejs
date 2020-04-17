<template>
  <div>
    <h1>Uh-Oh!</h1>
    <h3>It looks like youre experiencing some network issue</h3>
    <router-link :to="{ name: 'event-list' }">Go back to home</router-link>
  </div>
</template>
<script>
export default {
  props: {
    resource: {
      type: String,
      required: true
    }
  }
}
</script>
