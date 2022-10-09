<template>
  <div class="coment">
    <h1>komentar</h1>
    <form>
      <div>
        <label for="name">ketik nama:</label>
        <input placeholder="masukkan nama" id="name" name="name" required>
      </div>
      <div>
        <label for="age">umur:</label>
        <input placeholder="masukkan umur" type="number" v-model="age">
      </div>
      <div>
        <label for="komentar">komentar:</label>
        <input type="text" placeholder="masukkan komentar">
      </div>
      <button type="submit">simpan</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "ComentComponent",
  data() {
    return {
      age: "",
    }
  },
};
</script>

<style>
.coment {
  padding: 5px 20px;
  background-color: rgb(189, 189, 189);
  height: 280px;
}

.coment form {
  display: flex;
  flex-direction: column;
  text-align: justify;
  gap: 20px;
  width: 100px;
  margin: 0px 10px;
}
</style>
