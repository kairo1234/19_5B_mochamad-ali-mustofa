<template>
  <div class="Home">
    <BannerComponent />
    <div class="service">
      <h2>service</h2>
      <div class="list">
        <CardComponent v-for="(item, index) in services" :description="item.description" :imgUrl="item.imgUrl"
          :key="index" />
      </div>
    </div>
    <div class="coment">
      <div>
        <ComentComponent />
      </div>
    </div>
    <div class="medsos">
      <h2>media sosial</h2>
      <div class="lists">
        <MediaComponent v-for="(img, url) in mediasosial" :ImgUrl="img.ImgUrl" :key="url" />
      </div>
    </div>
  </div>
</template>

<script>
import BannerComponent from "@/components/BannerComponent.vue";
import CardComponent from "@/components/CardComponent.vue";
import ComentComponent from "@/components/ComentComponent.vue";
import MediaComponent from "@/components/MediaComponent.vue";
export default {
  name: "HomeView",
  components: { BannerComponent, CardComponent, ComentComponent, MediaComponent },
  data() {
    return {
      services: [
        {
          imgUrl: "https://cdn-icons-png.flaticon.com/128/870/870175.png",
          description: "layanan digital",
        },
        {
          imgUrl: "https://cdn-icons-png.flaticon.com/128/870/870175.png",
          description: "layanan email dan telepon",
        },
        {
          imgUrl: "https://cdn-icons-png.flaticon.com/128/870/870175.png",
          description: "layanan komunikasi forum",
        },
        {
          imgUrl: "https://cdn-icons-png.flaticon.com/128/870/870175.png",
          description: "layanan self-service",
        },
      ],
      mediasosial: [
        {
          ImgUrl: "https://cdn-icons-png.flaticon.com/128/1384/1384063.png",
        },
        {
          ImgUrl: "https://cdn-icons-png.flaticon.com/128/3128/3128304.png",
        },
        {
          ImgUrl: "https://cdn-icons-png.flaticon.com/128/3128/3128310.png",
        },
      ]
    };
  },
};
</script>

<style>
h2 {
  padding: 5px;
}
.Home .service {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.Home .service .list {
  padding: 10px 10px 20px 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
}
.Home .medsos .lists {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  padding: 10px;
}
</style>
