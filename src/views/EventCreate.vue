<template>
  <div>
    <h1>Create an event, {{ user.name }}</h1>
    <p>This event {{ user.id }}</p>
    <p>{{ getEventById(2) }}</p>
  </div>
</template>

<script>
import { mapState, mapGetters } from 'vuex'
export default {
  computed: {
    ...mapGetters(['getEventById']),
    ...mapState(['user', 'categories'])
  }
}
</script>

<style scoped></style>
