<template>
  <div class="container">
    <div class="row">
      <div class="col-md-4">
        <componentCard></componentCard>
      </div>
      <div class="col-md-4">
        <componentCard></componentCard>
      </div>
      <div class="col-md-4">
        <componentCard></componentCard>
      </div>
    </div>
  </div>
</template>

<script>
import componentCard from "./componentCard";
import Axios from "axios";

export default {
  name: "componentCardSection",
  components: {
    componentCard
  },

  data() {
    return {
      recipes: []
    };
  },

  mounted() {
    Axios.get(
      "https://cors-anywhere.herokuapp.com/http://www.recipepuppy.com/api"
    ).then(function(response) {
      this.recipes = response.data;
    });
  }
};
</script>
