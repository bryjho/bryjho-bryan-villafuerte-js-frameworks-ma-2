<template>
  <div class="card">
    <img class="card-img-top" src="recipeImg" alt="Card image cap" />
    <div class="card-body">
      <h5 class="card-title">{{ recipeTitle }}</h5>
      <p class="card-text">{{ recipeIngredients }}</p>
      <a href="recipeLink" class="btn btn-primary">View Recipe</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "componentCard",
  props: ["recipeImg", "recipeTitle", "recipeLink", "recipeIngredients"]
};
</script>
