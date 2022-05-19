<template>
  <div id="app">
    
    <PxHeader :links="links"></PxHeader>

    <router-view/>
  </div>
</template>

<script>
import PxHeader from '@/components/PxHeader.vue'

export default {
  name: "app",
  components: { PxHeader },

  data() {
    return {
      links: [
        {
          title: "Login",
          to: { name: "login" }
        },
      ]
    };
  }
};
</script>
