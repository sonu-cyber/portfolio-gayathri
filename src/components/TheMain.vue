<template>
  <div>
    <Body>
      <template v-slot:paraOne>
        <p>
          My name is Gayathri Raghuram. I am a Front End Developer. I am looking
          for opportunities to work remotely or on site or in a hybrid setting.
          I have 4+ years of experience working in the area of computer science.
          I have worked for 2 years as a Software Engineer & 2 years as an
          Adjunct Instructor in Computer science.
        </p>
      </template>
      <template v-slot:paraTwo>
        <p>
          I have a background in HTML, CSS, Javascript, GIT,Bootstrap, Tailwind
          CSS and I have worked with JS Frameworks like VueJs, NuxtJs, PINIA &
          consuming REST API’s. I have also worked with UI/UX design tools like
          Adobe Illustrator, Adobe XD, Sketch etc
        </p>
      </template>
      <template v-slot:paraThree>
        <p>
          I am looking for Front End Web Developer positions. I have trained in
          online courses with Udemy, Eduonix etc for the past 4 yrs and worked
          on projects on my own too. 
          I have worked on my own projects using the
          Fetch API, DOM Manipulation, Flexbox, Grid,Bootstrap, Tailwindcss, SASS(SCSS),media-Queries, Vue3,Vue Routing, Vuex, PINIA, NUXT,etc.
          I am familiar with ReactJs,React Hooks React Routing etc.
        </p>
      </template>
      <template v-slot:paraFour>
        <p>
          I have also worked on my own projects using the Fetch API, DOM Manipulation, Flexbox, Media-Queries, VueJs(Routing) etc. My projects are also available on my GITHUB repository
          https://github.com/sonu-cyber
        </p>
      </template>

      <template v-slot:paraFive>
        <p>
          I have used VueJs3 to develop this portfolio. I have also used component nesting,routing, props and slots including named slots in this project.
        </p>
      </template>
    </Body>

    <Footer class="contact">
      <template v-slot:footerSlot>
        <h3>Contact Me</h3>
        <ul class="contact">
          <li>Email:gayathriraghuram1@gmail.com</li>
          <li>Ph:+1 (617)-430-5548</li>
          <li>
            <img src="../assets/3-2-github-png-image_16x16.ico" /><span
              ><a
                href="https://github.com/sonu-cyber"
                target="_blank"
                alt="github"
                class="github-link"
                >GitHub</a
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
import Body from "../components/Body.vue";
import Footer from "../components/Footer.vue";

export default {
  components: { Body, Footer },

  data() {
    return {};
  },
  methods: {},
};
</script>

<style scoped></style>
