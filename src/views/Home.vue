<template>
  <div class="home">
    <div class="destingations">
      <div v-for="destination in destinations" :key="destination.name">
        <route-link :to="destination.slug"><h1>{{ destination.name }}</h1></route-link>
        <figure>
          <route-link :to="destination.slug">
            <img src="../assets/brazil.jpg" :alt="destination.name">
          </route-link>
        </figure>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import store from '@/store.js'

export default {
  name: 'Home',
  components: {
  },
  data () {
    return {
      destinations: store.destinations
    }
  },
  methods: {
    getPic (index) {
      return '../assets/' + index
    }
  }
}
</script>
<style scoped>
  .home {
    max-width: 1400px;
    margin: 0 auto;
  }
  .destingations {
    display: flex;
    justify-content: space-between;
  }
  .destingations img {
    width: 100%;
  }
</style>
