<template>
  <div>
      <Teams />
      <Register />
      <Reviews />
  </div>
</template>

<script>
import Register from "./Register.vue"
import Reviews from "./Reviews.vue"
import Teams from "./Teams.vue"
export default {
    components: {
        Register,
        Reviews,
        Teams
    }
}
</script>

<style>

</style>