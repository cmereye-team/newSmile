<template>
  <div class="main_banner">
    <banner class="banner">
      <template #title>
        聯絡我們
      </template>
    </banner>
  </div>
</template>
<script>
import Banner from "@/components/commom/head/Banner.vue";
export default {
  components: { Banner },
  data() {
    return {};
  },
  created() {},
  methods: {},
};
</script>
<style lang="scss" scoped>
@media (min-width: 768px) {
  .banner {
    background: url("https://static.cmereye.com/static/lkximg/smile_image/ContactUsBanner_pc.avif")
      no-repeat;
  }
}
@media (max-width: 768px) {
  .section {
    width: 100vw;
    margin: 0 auto;
    margin-bottom: 10vw;
  }
  .banner {
    background: url("https://static.cmereye.com/static/lkximg/smile_image/ContactUsBanner_mb.avif")
      no-repeat;
  }
}
</style>
