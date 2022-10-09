<template>
  <div class="card">
    <img :src="imgUrl" alt="image" />
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props: ["description", "imgUrl"],
};
</script>

<style>
.card {
  padding: 10px;
  margin: 0px 10px;
  background-color: rgb(189, 189, 189);
  height: 200px;
  width: 200px;
}
.card img {
  width: 100px;
}
</style>
