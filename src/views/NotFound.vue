<template>
  <div>
    <h1>Oops!</h1>
    <h3>The {{ resource }} doesnt exists!</h3>
    <router-link :to="{ name: 'route-list' }">Go back to home</router-link>
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
