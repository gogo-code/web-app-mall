<template>
  <h2>asfd</h2>
</template>

<script>
import HomeSwiper from './childComps/HomeSwiper'
import RecommendView from './childComps/RecommendView'
import { getHomeMultidata } from "network/home";
export default {
  name: "Home",
  data() {
    return {
      banners: [],
      recommends: [],
    };
  },
  created() {

    getHomeMultidata().then(res => {
      console.log(res.data.banner.list)
      this.banners = res.data.banner.list;
      this.recommends = res.data.recommend.list;
    });
  },
};
</script>

<style scoped>
</style>
