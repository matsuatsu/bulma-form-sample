<template>
  <div class="columns is-full">
    <SideMenu />
    <div class="column is-10 is-fullheight">
      <Clustering />
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import SideMenu from "~/components/SideMenu.vue";
import Clustering from "~/components/Clustering.vue";

export default {
  components: {
    Logo,
    SideMenu,
    Clustering
  },
  data() {
    return {
      n_cluster: 1
    };
  }
};
</script>

<style>
details {
  background: rgb(235, 235, 235);
  padding: 5px 10px 5px 10px;
  margin: 10px;
}
details > summary:focus {
  outline: none;
}
details > summary {
  cursor: pointer;
}

aside {
  background: rgb(235, 235, 235);
}
</style>
