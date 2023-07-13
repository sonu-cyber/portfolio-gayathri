<template>
  <div class="home">
    <PortfolioLinks :links="links" />
    <TheHome />
  </div>
</template>

<script>
import PortfolioLinks from "../components/PortfolioLinks.vue";
import TheHome from "../components/TheHome.vue";

export default {
  components: {
    PortfolioLinks,
    TheHome,
  },
  props: ["links"],

  data() {
    return {
      msg: "Returning the Lists",
    };
  },
};
</script>
