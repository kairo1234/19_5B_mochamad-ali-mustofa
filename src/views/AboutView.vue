<template>
  <div class="abouts">
    <div class="cards">
      <div class="lists">
        bussines adalah layanan digital yang menyediakan bisnis digital. saat ini layanan my bussines sudah tersebar ke seluruh indonesia agar bisa memenuhi kebutuhan masyatakat dan memperkenalkan produk kepada masyarakat. bussines juga membantu memperkenalkan prosuk ke masyarakat luar.
      </div>
      <div>
        <img src="https://tse2.mm.bing.net/th?id=OIP.xdAYNpQ2Xfv04f52rjWoSwHaD4&pid=Api&P=0" alt="image">
      </div>
    </div>
    <div class="medsos">
      <h2>media sosial</h2>
      <div class="lists">
        <MediaComponent v-for="(img, url) in mediasosial" :ImgUrl="img.ImgUrl" :key="url"/>
      </div>
    </div>
  </div>
</template>

<script>
import MediaComponent from '@/components/MediaComponent.vue'; 

export default {
    name: "AboutView",
    components: { MediaComponent },
    data() {
        return {
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
}
</script>
<style>
.abouts {
  padding: 10px 10px;
}
.about .cards {
  display: flex;
}
.abouts .cards .lists {
  justify-content: left;
}
.abouts img {
  width: 300px;
}
.abouts .medsos .lists {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  padding: 10px;
}
.abouts .medsos .lists img {
  width: 30px;
}
</style>