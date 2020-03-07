<template>
  <div id="app">
    <componentHeader></componentHeader>
    <componentCardSection></componentCardSection>
  </div>
</template>

<script>
import componentHeader from "./components/componentHeader.vue";
import componentCardSection from "./components/componentCardSection.vue";

export default {
  name: "App",
  components: {
    componentHeader,
    componentCardSection
  }
};
</script>
