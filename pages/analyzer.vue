<template>
  <div class="section">
    <h1 class="title">Analyzer</h1>
    <hr />
    <div class="grid">
      <div @click="$router.push('/clustering')">
        <p class="title">Clustering</p>
        <p class="subtitle">Subtitle</p>
      </div>
      <div>
        <p class="title">One</p>
        <p class="subtitle">Subtitle</p>
      </div>
      <div>
        <p class="title">One</p>
        <p class="subtitle">Subtitle</p>
      </div>
      <div>
        <p class="title">One</p>
        <p class="subtitle">Subtitle</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(25em, 1fr));
  grid-template-rows: repeat(auto-fit, minmax(200px, 1fr));
  grid-auto-rows: 1fr;
  grid-gap: 0.8em;
}

.grid > div {
  box-shadow: 0px 0px 5px #312d2d;
  border-radius: 10px;
  overflow: auto;
  padding: 1em;
  margin: 0.5em;
}

.grid > div:hover {
  box-shadow: 0px 0px 5px #f14c2e;
}
</style>
