<script>
export default {
  props: {
    links: {
      type: Object,
    },
    title: {
      type: String,
    },
    id: {
      type: Number,
    },
  },
  data() {
    return {
      title: "Portfolio Links",
      show: false,
    };
  },
  methods: {
    changeTitle: function () {
      this.title = "Portfolio Details";
    },
    showLinks: function () {
      this.show = !this.show;
    },
  },
};
</script>

<template>
  <div class="port-folio">
    <h3 @click="changeTitle">{{ title }}</h3>

    <ul v-if="show">
      <li v-for="link in links" :key="link.id">
        <a v-bind:href="link.url" target="_blank" rel="noopener" class="link">
          {{ link.url }}
        </a>
      </li>
    </ul>
    <button class="port-btn" @click="showLinks">Portfolio Links</button>
  </div>
</template>

<style scoped></style>
