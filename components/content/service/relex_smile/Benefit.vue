<template>
  <div class="benefit section pc_page_container">
    <div class="flex justify-center md:mt-28 mt-10 page_container">
      <h2>SMILE 微笑激光矯視的好處</h2>
    </div>
    <div class="benefit_content">
      <ul
        class="benefit_list flex flex-col items-start justify-start page_container"
      >
        <li v-for="(benefitItem, index) in benefitList" :key="index">
          <img :src="benefitItem.index" alt="" class="index" />
          <p>{{ benefitItem.des }}</p>
        </li>
      </ul>
      <img
        class="benefit_img benefit_eye"
        src="@/asset/image/service/relex_smile/benefit_eye.jpg"
        alt=""
      />
      <img
        class="benefit_img benefit_light"
        src="@/asset/image/service/relex_smile/benefit_light.jpg"
        alt=""
      />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      benefitList: [
        {
          index: require("@/asset/image/service/relex_smile/benefit_index1.svg"),
          des: "無需製造角膜瓣",
        },
        {
          index: require("@/asset/image/service/relex_smile/benefit_index2.svg"),
          des: "最快術後翌日生活、工作",
        },
        {
          index: require("@/asset/image/service/relex_smile/benefit_index3.svg"),
          des: "4至5分鐘",
        },
        {
          index: require("@/asset/image/service/relex_smile/benefit_index4.svg"),
          des: "減低術後眼乾及感染情況",
        },
        {
          index: require("@/asset/image/service/relex_smile/benefit_index5.svg"),
          des: "傷口只有約2mm",
        },
        {
          index: require("@/asset/image/service/relex_smile/benefit_index6.svg"),
          des: "視力改善顯著",
        },
      ],
    };
  },
  created() {},
  methods: {},
};
</script>

<style lang="scss" scoped>
@media screen and (min-width: 768px) {
  .pc_page_container {
    max-width: 1280px !important;
    margin-left: auto;
    margin-right: auto;
    padding-left: 1rem;
    padding-right: 1rem;
    width: 100%;
  }
  h2 {
    font-size: 25px;
  }
  .section {
    margin-bottom: 0;
  }
  .benefit_content {
    position: relative;
    .benefit_img {
      position: absolute;
    }
    .benefit_eye {
      top: -1vw;
      right: 2vw;
      z-index: 2;
      height: auto;
    }
    .benefit_light {
      top: 10vw;
      right: 0;
      z-index: 1;
      height: auto;
    }
  }
  .benefit_list {
    background: url(/_nuxt/asset/image/service/relex_smile/benefit_bg.png);
    background-repeat: no-repeat;
    background-size: cover;
    text-align: right;
    background-position-y: 3vw;
    margin-right: 304px;
    height: auto;
    margin-top: 3vw;
    li {
      margin: 0.5vw 0;
      z-index: 11;
      p {
        font-family: "Noto Sans JP";
        font-style: normal;
        font-weight: 300;
        font-size: 17px;
        line-height: 31px;
        letter-spacing: 0.1em;
        color: #000000;
      }
      img {
        height: 90px;
      }
    }
    li:nth-child(1) {
      margin-left: 0vw;
    }
    li:nth-child(2) {
      margin-left: 165px;
    }
    li:nth-child(3) {
      margin-left: 32px;
    }
    li:nth-child(4) {
      margin-left: 402px;
    }
    li:nth-child(5) {
      margin-left: 140px;
    }
    li:nth-child(6) {
      margin-left: 520px;
      padding-bottom: 123px;
    }
  }
}

@media screen and (max-width: 768px) {
  .section {
    margin-bottom: 0;
  }
  .benefit_content {
    position: relative;
    .benefit_img {
      position: absolute;
    }
    .benefit_eye {
      top: -1vw;
      right: 2vw;
      z-index: 2;
      height: auto;
    }
    .benefit_light {
      top: 10vw;
      right: 0;
      z-index: 1;
      height: auto;
    }
  }
  h2 {
    font-size: 16px;
  }
  h2::before {
    width: 14vw !important;
    height: 0;
    border-top: 1px solid #dfdfdf;
    left: -14vw !important;
  }
  h2::after {
    width: 14vw !important;
    height: 0;
    border-top: 1px solid #dfdfdf;
    right: -14vw !important;
  }
  .benefit_content .benefit_eye {
    width: 90%;
    height: unset;
    right: 3vw !important;
    top: -49vw !important;
  }
  .benefit_list {
    background: url(("https://static.cmereye.com/imgs/2022/12/a2c6adf210ffc920.jpg"))
      no-repeat;
    margin-top: 50vw;
    height: 106vw;
    background-position: center;
    background-position-x: 0;
    margin-bottom: 58px;
    li {
      img {
        height: 11vw;
      }
      margin-bottom: 10px;
      p {
        font-family: "Noto Sans JP";
        font-style: normal;
        font-weight: 300;
        font-size: 15px;
        text-align: right;
        letter-spacing: 0.1em;
        color: #000000;
        white-space: pre;
      }
    }
  }
  .benefit_list li:nth-child(1) {
    margin-left: 2vw;
  }
  .benefit_list li:nth-child(2) {
    margin-left: 18vw;
    z-index: 11;
  }
  .benefit_list li:nth-child(3) {
    margin-left: 7vw;
  }
  .benefit_list li:nth-child(4) {
    margin-left: 39vw;
    margin-top: -3vw;
    z-index: 11;
  }
  .benefit_list li:nth-child(5) {
    margin-left: 18vw;
    margin-top: -2vw;
  }
  .benefit_list li:nth-child(6) {
    margin-left: 39vw;
  }
  .benefit_content .benefit_light {
    top: -14vw;
    right: 0;
    z-index: 1;
    height: 60vw;
  }
}
</style>
