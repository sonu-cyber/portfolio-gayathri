<template>
  <div class="contact-view">
    <h3>Contact Me</h3>
    <ul>
      <li>Email:{{ email }}</li>
      <li>Ph:{{ phone }}</li>
      <li>
        <span>github url:{{ url }}</span>
      </li>
    </ul>
  </div>
  <div>
    <Footer>
      <template v-slot:footerSlot>
        <h3>Contact Me</h3>
        <ul class="contact">
          <li>Email:gayathriraghuram1@gmail.com</li>
          <li>Ph:+1 (617)-430-5548</li>

          <li>
            <img
              src="../assets/3-2-github-png-image_16x16.ico"
              alt="github"
            /><span
              ><a
                href="https://github.com/sonu-cyber"
                target="_blank"
                alt="github"
                class="github-link"
              >
                GitHub</a
              ></span
            >
            <img
              src="../assets/linkedin-icon-no-background-19.jpg"
              width="300px"
              height="300px"
              alt="LinkedIn"
            /><span>
              <a
                href="https://linkedin.com/in/gayathriraghuram/"
                target="_blank"
                alt="LinkedIn"
                class="linkedin-link"
              >
                LinkedIn
              </a></span
            >
          </li>
        </ul>
      </template>
    </Footer>
  </div>
</template>

<script>
import Footer from "../components/Footer.vue";
export default {
  components: { Footer },
  data() {
    return {
      email: "gayathriraghuram1@gmail.com",
      phone: "+1-617-430-5548",
      url: "https://github.com/sonu-cyber",
      show: true,
    };
  },
};
</script>

<style scoped></style>
