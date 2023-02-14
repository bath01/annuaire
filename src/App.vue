<template>
  <h1 class="titre">Annuaire Orange Digital Academie</h1>
  
  <RechercherSearch/>

  <div id="app">
    <input type="text" v-model="search" />
    <div v-for="post in filteredPosts" :key="post.id">
      <Post-vue :post="post"></Post-vue>
    </div>
  </div>
  <div class="container">
    <!-- <card-annuaire />
    <card-annuaire />
    <ca-->
  </div>
</template>

<script>
import PostVue from "./components/PostVue.vue";
import RechercherSearch from './components/RechercherSearch.vue';
// import CardAnnuaire from "./components/CardAnnuaire.vue";

export default {
  name: "App",
  components: {
    PostVue,
    RechercherSearch,
    // CardAnnuaire,
  },
  data(){
    return{

    }
  },
  methods:{
    async
  }
  // data() {
  //   return {
  //     search: "",
  //     posts: [
  //       {
  //         id: 1,
  //         title: "Post 1",
  //         body: "Vue.js is cool",
  //       },
  //       {
  //         id: 2,
  //         title: "Post 2",
  //         body: "JavaScript  is cool",
  //       },
  //     ],
  //   };
  // },
  // computed: {
  //   filteredPosts() {
  //     return this.posts.filter((post) =>
  //       post.body.toLowerCase().includes(this.search.toLowerCase())
  //     );
  //   },
  // },
};
</script>

<style lang="scss">
.titre {
  color: black;
}
.container {
  display: flex;
  flex-wrap: wrap;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
