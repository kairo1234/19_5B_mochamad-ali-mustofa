<template>
    <div class="medsos">
        <img :src="ImgUrl" alt="media sosial">
    </div>
</template>
<script>
export default {
    name: "MediaComponent",
    props: ["ImgUrl"],
};
</script>

<style>
.medsos {
    background-color: rgb(255, 0, 0);
}
.medsos img {
    width: 30px;
    padding: 0px 0px;
    margin: 0px 0px;
}
</style>