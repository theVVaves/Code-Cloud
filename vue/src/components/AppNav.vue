<template>
  <div id="nav">
    <div class="title-logo">
      <img
        src="@/assets/logo/cloudcode.svg"
        alt="CodeCatalog Logo"
        v-on:click.prevent="goHome"
      />
      <h5 v-on:click.prevent="goHome">Code Cloud</h5>
    </div>
    <catalog-search />

    <div class="menu-btns">
      <router-link v-bind:to="{ name: 'home' }" v-on:click="retrieveExample"
        >Home
      </router-link>
      <router-link v-bind:to="{ name: 'Catalog' }">Catalog</router-link>
      <router-link v-bind:to="{ name: 'addExample' }">Add Code</router-link>
      <router-link
        v-bind:to="{ name: 'logout' }"
        v-if="$store.state.token != ''"
      >
        Logout</router-link
      >
      <router-link
        v-bind:to="{ name: 'logout' }"
        v-if="$store.state.token == ''"
      >
        Log In</router-link
      >
      <i
        v-on:click="
          $router.push({
            name: 'ManageProfile',
          })
        "
        class="fa-solid fa-circle-user"
      ></i>
    </div>
  </div>
</template>

<script>
import CatalogSearch from "@/components/CatalogSearch";

export default {
  components: {
    CatalogSearch,
  },
  methods: {
    retrieveExample() {},
    goHome() {
      this.$router.push({ path: "/" });
    },
  },
};
</script>

<style scoped>
#nav {
  position: fixed;
  width: 100%;
  height: 85px;

  box-shadow: 0 2px 2px rgba(0, 0, 0, 0.4);
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  /* background:url(../assets/cloudbannerfooter/cloudbannernav.svg); */
  backdrop-filter: blur(7px);
  background-color: rgba(158, 154, 154, 0.4); /* Black w/opacity/see-through */

  font-size: 1.2rem;
  color:black;
  font-weight:bold;
}

.title-logo {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.title-logo h5 {
  font-weight: bold;
  letter-spacing: 3px;
  margin-bottom: 0;
}

.title-logo > * {
  cursor: pointer;
}

.title-logo img {
  width: 100px;
  margin-right: 5px;
}

.menu-btns {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}

a {
  color: rgb(0, 0, 0);
}
a:hover {
  color: black;
  text-decoration-line: none;
  text-shadow:  0 0 15px rgb(0, 150, 255);
}

.menu-btns i:hover {
  box-shadow: 0 0 10px 5px rgb(0, 150, 255);
  border-radius: 5000px;
}

router-link {
  width: fit-content;
}
</style>
