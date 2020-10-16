<template>
  <div class="about">
    <h1>This is an about page</h1>
    <aboutUs msg="somethign"></aboutUs>
  </div>
</template>

<script>
import aboutUs from '@/components/aboutUs.vue'
export default {
  name: 'About',
  components: {
    aboutUs
  }
}
</script>
