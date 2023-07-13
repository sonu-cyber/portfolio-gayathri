<script>
/*  */
import TheMain from "../components/TheMain.vue";

export default {
  props: {
    titleAbout: {
      type: String,
    },
  },
  components: { TheMain },
  data() {
    return {
      titleAbout: "My Experience",
    };
  },
};
</script>

<template>
  <div class="about">
    <h3>{{ titleAbout }}</h3>
    <TheMain />
  </div>
</template>

<style>
/* @media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  } 
}*/
</style>
