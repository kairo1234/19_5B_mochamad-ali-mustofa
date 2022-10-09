<template>
  <div class="navigation">
    <img src="../assets/my-business.png" alt="my bussines">
    <router-link to="/">Home</router-link>
    <router-link to="/About">About</router-link>
  </div>
</template>

<script>
export default {
  name: "NavigationComponent",
};
</script>

<style>
.navigation {
  display: flex;
  align-items: center;
  gap: 20px;
  background-color: rgb(255, 0, 0);
  padding: 10px 20px;
}
.navigation img {
  height: 50px;
}
.navigation a {
  font-size: 1.2em;
  text-decoration: none;
}
.navigation a:hover {
  font-weight: 700;
}
</style>
