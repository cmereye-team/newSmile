<template>
  <div class="main_banner">
    <banner class="banner">
      <template v-slot:title class="title">
        <div class="pcShow">
          <p style="font-size: 28px">CMER CLEAR-Vision</p>

          <span>(C-MER Lens Exchange Achieving Renewed Vision)</span>
        </div>
        <div class="mbShow banner_serve">
          <p>CMER CLEAR-Vision</p>
          <span
            >(C-MER Lens Exchange Achieving<br />
            Renewed Vision)</span
          >
        </div>
      </template>
      <template v-slot:des>
        <div class="pcShow">
          坊間稱之為人工晶體置換術。透過更換人工晶體，致力為客人視野帶來煥然一新的感覺，一次過解決近視、遠視、散光、老花等問題。
          希瑪微笑矯視中心針對客人眼睛實際狀況、職業、生活需要等因素，度身訂造矯視方案；專業咨詢過後，眼科專科醫生按客人視力需求選取及植入合適之人工晶體，以替代原有已老化和混濁
        </div></template
      >
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
@media screen and (max-width: 768px) {
  .banner_serve {
    margin-bottom: 49px;
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 700;
      font-size: 20px;
      line-height: 23px;
      /* or 115% */
      white-space: pre;
      letter-spacing: 0.08em;

      background: linear-gradient(90.24deg, #4570b6 12.21%, #81dbec 87.2%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
      padding-bottom: 5px;
      padding-top: 0;
    }
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 300;
      font-size: 12px;
      line-height: 23px;
      letter-spacing: 0.08em;
      background: linear-gradient(90.24deg, #4570b6 12.21%, #81dbec 87.2%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
    }
  }
  .section {
    .des_box {
      width: 60.5vw !important;
      letter-spacing: 0.2vw;
      margin-top: 5vw;
    }
  }
  .banner {
    background-image: url("https://static.cmereye.com/imgs/2023/03/499555fcd696e4f1.jpg");

    background-size: 100%;
    width: 100vw;
    margin: 0 auto;
    margin-bottom: 10vw;
  }
}

@media screen and (min-width: 768px) {
  .banner {
    background-image: url("https://static.cmereye.com/imgs/2023/03/9a5638da4be73377.jpg");
    // background-position-x: right !important;
  }
}
</style>
