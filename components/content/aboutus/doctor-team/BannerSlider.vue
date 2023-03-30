<template>
  <div class="main_banner">
    <banner class="banner"></banner>
  </div>
</template>
<script>
import Banner from "@/components/commom/head/Banner.vue";
export default {
  components: { Banner },
  data() {
    return {};
  },
  created() { },
  methods: {}
};
</script>
<style lang="scss" scoped>
@media (min-width: 768px){
  .banner {
  background: url("https://static.cmereye.com/imgs/2022/12/d8af6e40054d2684.jpg") no-repeat;
}
}
@media (max-width: 768px){
  .section{
    width: 100vw;
    margin:0 auto;
    margin-bottom: 10vw;
  }
  .banner {
  background: url("https://static.cmereye.com/imgs/2022/12/efa3ddacc9443355.png") no-repeat;
}
}
</style>