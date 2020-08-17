<template>

</template>

<script>
import {Swiper,SwiperItem} from 'components/common/swiper'
export default {
  name:'',
  props: {
    banners: {
      type:Array,
      default() {
        return []
      }
    }
  },
  data(){
    return {

    }
  },
  components: {
    Swiper,
    SwiperItem
  }
}
</script>

<style scoped>

</style>
