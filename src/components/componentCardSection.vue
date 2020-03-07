<template>
  <div class="container">
    <div class="row">
      <div class="col-md-4">
        <componentCard></componentCard>
      </div>
    </div>
  </div>
</template>

<script>
import componentCard from "./componentCard";

export default {
  name: "componentCardSection",
  components: {
    componentCard
  },
}
</script>
