<template>
  <div class="fit">
    <div class="section page_container">
      <h3 class="gradient_title_bg">你適合接受SMILE 微笑矯視嗎？</h3>
      <div class="fit_des flex justify-between pcShow">
        <ul class="fit_des_first">
          <li v-for="(item1, index) in fitList1" :key="index">
            <strong>{{ item1 }}</strong>
            <div v-html="text"></div>
          </li>
        </ul>
        <ul>
          <li v-for="(item2, index) in fitList2" :key="index">
            <strong>{{ item2 }}</strong>
          </li>
        </ul>
      </div>
      <div class="fit_des flex justify-between mbShow">
        <div v-swiper:mySwiper="swiperOptionMb" class="swiperWrap">
          <div class="swiper-wrapper">
            <div class="swiper-slide">
              <ul>
                <li v-for="(item1, index) in fitList1" :key="index">
                  <strong>{{ item1 }}</strong>
                  <div v-html="text"></div>
                </li>
              </ul>
            </div>
            <div class="swiper-slide fitList2">
              <ul>
                <li v-for="(item2, index) in fitList2" :key="index">
                  <strong>{{ item2 }}</strong>
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- <ul>
          <li v-for="(item2,index) in fitList2" :key="index"><strong>{{item2}}</strong></li>
        </ul> -->
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      swiperOptionMb: {
        centeredSlides: true,
        spaceBetween: 10,
        slidesPerView: "1",
        pagination: {
          el: ".swiper-pagination",
          dynamicBullets: true,
        },
      },
      fitList1: [
        "1,000度以下近視，\n500度以下散光眼球 ",
        "發育成熟，近視度數穩定 ",
        " 角膜厚度正常",
        "角膜沒受感染，\n例如發炎或曾受傷",
      ],
      fitList2: [
        "沒有患上眼疾，\n如青光眼或視網膜疾病 ",
        "沒有患上自體免疫疾病，\n如風濕性關節炎或紅斑狼瘡 ",
        " 不需要長期服用類固醇",
        " 非懷孕",
      ],
    };
  },
  created() {
    //    this.fitList1.replace(/\n/g, '<br>')
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@media screen and (min-width: 768px) {
  h2 {
    font-size: 25px;
  }
  .fit {
    max-width: 1280px;
    margin: auto;
    background-image: url("@/asset/image/service/relex_smile/fit_bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    height: 44vw;
    .section {
      margin-top: 0;
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      padding-top: 5vw;
      h3 {
        font-size: 25px;
        margin-bottom: 4.5vw;
        margin-right: 200px;
      }
      .fit_des_first {
        margin-right: 100px;
      }
      .fit_des {
        margin-left: 5vw;
        ul {
          li {
            white-space: pre-wrap;
            margin-bottom: 4vw;
            position: relative;
            z-index: 9;
            strong {
              font-family: "Noto Sans JP";
              font-style: normal;
              font-weight: 400;
              font-size: 17px;
              line-height: 25px;
              /* or 167% */

              letter-spacing: 0.1em;

              color: #000000;
            }
            &::before {
              content: " ";
              position: absolute;
              background: rgba(129, 219, 236, 0.3);
              width: 3vw;
              height: 3vw;
              border-radius: 100%;
              top: -1.2vw;
              left: -1.3vw;
              z-index: -1;
            }
          }
          li:nth-child(1) {
            margin-left: -2vw;
          }
          li:nth-child(2) {
            margin-left: 0;
          }
          li:nth-child(3) {
            margin-left: 2vw;
          }
          li:nth-child(4) {
            margin-left: 4vw;
          }
        }
        ul:nth-child(2) {
          margin-top: 5vw;
        }
      }
    }
  }
}

@media screen and (max-width: 768px) {
  .fitList2 ul li:nth-child(2) {
    white-space: break-spaces !important;
  }
  .fit {
    background-image: url("https://static.cmereye.com/imgs/2022/12/a8f5b0b92f86d0e6.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    height: 84vw;
    position: relative;
    .section {
      margin-top: 0;
      padding-left: 46%;
      padding-top: 5vw;
      h3 {
        padding: 14px;
        position: absolute;
        right: 0;
        font-family: "Noto Sans JP";
        font-style: normal;
        font-weight: 500;
        font-size: 13px;
        line-height: 5px;
        /* or 38% */

        text-align: center;
        letter-spacing: 0.1em;

        color: #ffffff;
      }
      .fit_des {
        margin-left: 29vw;
        margin-top: 71px;
        ul {
          li {
            font-family: "Noto Sans HK";
            font-style: normal;
            font-weight: 400;
            font-size: 15px;
            line-height: 20px;
            /* or 62% */
            letter-spacing: 0.1em;
            color: #000000;
            // white-space: nowrap;
            margin-bottom: 4vw;
            position: relative;
            z-index: 9;
            &::before {
              content: " ";
              position: absolute;
              background: rgba(129, 219, 236, 0.3);
              width: 6vw;
              height: 6vw;
              border-radius: 100%;
              top: -1.2vw;
              left: -1.3vw;
              z-index: -1;
            }
          }
          li:nth-child(1) {
            margin-left: 0vw;
          }
          li:nth-child(2) {
            margin-left: 3vw;
          }
          li:nth-child(3) {
            margin-left: 6vw;
          }
          li:nth-child(4) {
            margin-left: 8vw;
          }
        }
        ul:nth-child(2) {
          margin-top: 5vw;
        }
      }
    }
  }
  .fit::before {
    position: absolute;
    content: "";
    width: 12.5vw;
    height: 6.7vw;
    background-image: url(https://static.cmereye.com/imgs/2022/12/43871fde827f43df.png);
    bottom: 13vw;
    /* left: 0; */
    right: 16vw;
    /* top: 0; */
    background-size: 100%;
    background-repeat: no-repeat;
    -webkit-animation: translateX 1s ease-in-out alternate infinite;
    animation: translateX 1s ease-in-out alternate infinite;
  }
}
</style>
