<template>
  <main>
    <!-- Contenuto sito -->
    <div class="container">&#8674; Content goes here &#8672;</div>
  </main>
</template>

<script>
export default {
  name: "MainComponent",
};
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";

main {
  background-color: $bg-main;
  color: $txt-main;
  padding-top: 50px;
  padding-bottom: 50px;

  .container {
    font-size: 1.2rem;
  }
}
</style>
