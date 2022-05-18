<template xmlns="http://www.w3.org/1999/html">
  <div class="top-0 left-0 border-l-8 border-r-8 border-t-8 border-white">
    <nuxt-link to="/">
      <div class="flex justify-center">
        <img src="/logo.jpeg"/>
      </div>
    </nuxt-link>
    <ul class="flex justify-around border-t-8 border-white py-2">
      <li>
        <nuxt-link to="/" :class="$nuxt.$route.path === '/' ? 'text-purple-300' : 'text-pink-50'">
          <i>Home</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/artists" :class="$nuxt.$route.path === '/artists' ? 'text-purple-300' : 'text-pink-50'">
          <i>Artists</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/events" :class="$nuxt.$route.path === '/events' ? 'text-purple-300' : 'text-pink-50'">
          <i>Events</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/studio" :class="$nuxt.$route.path === '/studio' ? 'text-purple-300' : 'text-pink-50'">
          <i>Studio</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/contact" :class="$nuxt.$route.path === '/contact' ? 'text-purple-300' : 'text-pink-50'">
          <i>Contact</i>
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    selected: { type: String, default: '' }
  }
}
</script>

<style scoped>

</style>
