<script>
import { RouterLink, RouterView } from "vue-router";
import Body from "./components/Body.vue";
import ContactView from "./views/ContactView.vue";

export default {
  name: "App",
  components: {},
  data() {
    return {
      links: [
        {
          id: this.displayId(),
          url: "https://portfolio-gayathri.netlify.app",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://github.com/sonu-cyber",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://github.com/sonu-cyber/weather-api-vue",
          show: true,
        },
        {
          id: this.displayId(),
          url: "https://github.com/sonu-cyber/messari_crypto_vue",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://dojo-nuxt.netlify.app",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://pinia-task.netlify.app/",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://simple-port-folio.netlify.app",
          show: true,
        },
        {
          id: this.displayId(),
          url: "https://www.linkedin.com/in/gayathriraghuram",
          show: true,
        },
        {
          id: this.displayId(),
          url: "https://weather-api-proj.netlify.app",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://cryptonator-api-proj.netlify.app",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://grid-port.netlify.app",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://nasa-apod-proj.netlify.app",
          show: true,
        },

        {
          id: this.displayId(),
          url: "https://trillo-proj.netlify.app",
          show: true,
        },
      ],
    };
  },
  methods: {
    goHome() {
      this.$router.push({ name: "home" });
    },
    goAbout() {
      this.$router.push("/about");
    },
    goForward() {
      this.$router.go(1);
    },
    goBack() {
      this.$router.go(-1);
    },
    updateTitle(e) {
      console.log("event", e);
    },
    displayId() {
      console.log("You clicked display");
      return (this.id = Math.floor(Math.random() * 15));
    },
  },
};
</script>

<template>
  <div class="header">
    <nav>
      <RouterLink class="router-link" to="/">Home</RouterLink>

      <RouterLink class="router-link" to="/about">About</RouterLink>

      <RouterLink class="router-link" to="/contact">Contact</RouterLink>
      <!--Navigation controls-->
      <!-- <h4>Navigation controls</h4> -->
      <ul class="router-link">
        <li><button class="btn" @click="goForward">Go Forward</button></li>
        <li><button class="btn" @click="goBack">Go Back</button></li>
      </ul>
    </nav>

    <!-- </nav> -->

    <RouterView :links="links" @changeTitle="updateTitle($event)" />
  </div>

  <ContactView />
</template>

<style scoped></style>
