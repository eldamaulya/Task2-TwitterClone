<script>
import Navbar from './components/Navbar.vue'
import Foto from './assets/selena.jpg'
import InputTweet from './components/InputTweet.vue'

export default {
  provide() {
    return {
      fullname: 'Elda Qotul Maulya',
      username: '@eldamaulya',
      profile: Foto
    }
  },
  components: {
    Navbar, InputTweet
  }
}
</script>

<template>
 <Navbar />

 <InputTweet />
</template>

<style>

</style>
