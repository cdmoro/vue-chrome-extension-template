<template lang="pug">
    div
      button(@click="tab") New tab
</template>
<script>
export default {
  methods: {
    tab() {
      chrome.tabs.create({ url: "pages/app.html" });
    }
  }
};
</script>
<style lang="scss">
div {
  color: blue;
}
</style>