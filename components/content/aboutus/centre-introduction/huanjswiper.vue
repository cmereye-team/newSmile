<template>
  <div class="bc">
    <div class="firstDiv page_container">
      <div class="centerDiv">
        <div class="thumb-example">
          <!-- 大轮播图 -->
          <div
            class="swiper gallery-top"
            v-swiper:swiperTop="swiperOptionTop"
            ref="swiperTop"
          >
            <div class="swiper-wrapper">
              <div class="swiper-slide slide-1"></div>
              <div class="swiper-slide slide-2"></div>
              <div class="swiper-slide slide-3"></div>
              <div class="swiper-slide slide-4"></div>
              <div class="swiper-slide slide-5"></div>
            </div>
          </div>
          <!-- 小缩略图 -->
          <div
            class="swiper gallery-thumbs"
            v-swiper:swiperThumbs="swiperOptionThumbs"
            ref="swiperThumbs"
          >
            <div class="swiper-wrapper">
              <div class="swiper-slide slide-1"></div>
              <div class="swiper-slide slide-2"></div>
              <div class="swiper-slide slide-3"></div>
              <div class="swiper-slide slide-4"></div>
              <div class="swiper-slide slide-5"></div>
            </div>
          </div>
          <div class="swiper-button-prev swiper-button-prev1"></div>
          <div class="swiper-button-next swiper-button-next1"></div>
        </div>
      </div>
    </div>
    <div class="text_ev page_container">
      <div class="box">
        <h3>中心環境舒適寬敞、地點便利</h3>
        <p>
          希望為客人提供安心自在的優質矯視服務，我們亦著重整體感官體驗，位於尖沙咀
          K11 ATELIER
          的旗艦店更配合時尚、寬敞及醉人海景，同樣配備齊全設備，致力提供最舒適、專業及優質的矯視服務。
        </p>
        <div class="address_box">
          <div class="address">
            <img
              src="https://static.cmereye.com/imgs/2023/03/c83a4a5880ab1940.png"
              alt=""
            />
            <p>中環</p>
          </div>
          <div class="address">
            <img
              src="https://static.cmereye.com/imgs/2023/03/c83a4a5880ab1940.png"
              alt=""
            />
            <p>銅鑼灣</p>
          </div>
          <div class="address">
            <img
              src="https://static.cmereye.com/imgs/2023/03/c83a4a5880ab1940.png"
              alt=""
            />
            <p>銅鑼灣</p>
          </div>
          <div class="address">
            <img
              src="https://static.cmereye.com/imgs/2023/03/c83a4a5880ab1940.png"
              alt=""
            />
            <p>尖沙咀</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "image",

  data() {
    return {
      swiperOptionTop: {
        loop: true,
        autoplay: true,
        loopedSlides: 8, // looped slides should be the same
        spaceBetween: 10,
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
      swiperOptionThumbs: {
        autoplay: true,
        loop: true,
        loopedSlides: 8, // looped slides should be the same
        spaceBetween: 0,
        centeredSlides: true,
        slidesPerView: "auto",
        touchRatio: 0.2,
        slideToClickedSlide: true,
        // slidesPerView: 3,
      },
    };
  },

  mounted() {
    this.$nextTick(() => {
      const swiperTop = this.swiperTop;
      const swiperThumbs = this.swiperThumbs;
      swiperTop.controller.control = swiperThumbs; //控制缩略图和轮播图联动
      swiperThumbs.controller.control = swiperTop;
    });
  },
};
</script>

<style lang="scss" scoped>
.slide-1 {
  background-image: url("https://static.cmereye.com/imgs/2023/03/c84f05c91befdb22.jpg");
}
.slide-2 {
  background-image: url("https://static.cmereye.com/imgs/2023/03/4f7d2ce27afb7c2f.jpg");
}
.slide-3 {
  background-image: url("https://static.cmereye.com/imgs/2023/03/8654b03f75e2cd4b.jpg");
}
.slide-4 {
  background-image: url("https://static.cmereye.com/imgs/2023/03/eb3214d4994e6988.jpg");
}
.slide-5 {
  background-image: url("https://static.cmereye.com/imgs/2023/03/990a811af868c7ed.jpg");
}
@media screen and (min-width: 768px) {
  .box:nth-child(1) img {
    height: unset;
  }
  .swiper-button-prev,
  .swiper-container-rtl .swiper-button-next {
    left: -61px;
    right: auto;
    background-image: url("https://static.cmereye.com/imgs/2023/03/bcc35245d4a0fe42.png");
  }
  .swiper-button-next,
  .swiper-container-rtl .swiper-button-prev {
    right: -61px;
    left: auto;
    background-image: url("https://static.cmereye.com/imgs/2023/03/c1cc233620b64f31.png");
  }
  .swiper-button-prev,
  .swiper-button-next {
    top: 64%;
  }
  .address_box {
    margin-top: 40px;
    display: flex;
    justify-content: space-evenly;
  }
  .address {
    p {
      margin-left: 10px;
    }
    display: flex;
    align-items: center;
  }
  .text_ev {
    .box {
      margin: 0 174px;
    }
    h3 {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 500;
      font-size: 23px;
      line-height: 52px;
      /* or 43% */
      letter-spacing: 0.1em;
      margin-top: 32px;
      color: #4570b6;
    }
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 300;
      font-size: 20px;
      line-height: 42px;
      /* or 43% */
      color: #6d6e71;
      letter-spacing: 0.1em;
    }
  }
  .firstDiv {
    height: 860px;
    position: relative;
    background: linear-gradient(180deg, #fff 64%, #d7eaf3 0);
  }

  .centerDiv {
    width: 900px;
    height: 800px;
    position: absolute;
    /* left: 510px; */
    top: 200px;
    left: 0;
    right: 0;
    /* display: flex; */
    /* flex-direction: column; */
    margin: auto;
    text-align: center;
  }

  .thumb-example {
    height: 580px;
    background-color: transparent;
  }

  .swiper-slide {
    background-size: cover;
    background-position: center;
  }
  .gallery-top {
    height: 80%;
    width: 100%;
  }
  .gallery-thumbs {
    height: 20%;
    box-sizing: border-box;
    padding: 10px 0;
  }
  .gallery-thumbs .swiper-slide {
    width: 20%;
    height: 100%;
  }
  .gallery-thumbs .swiper-slide-active {
    opacity: 1;
  }
}
@media screen and (max-width: 768px) {
  .swiper-button-prev,
  .swiper-container-rtl .swiper-button-next {
    left: -26px;
    right: auto;
    background: url("https://static.cmereye.com/imgs/2023/03/bcc35245d4a0fe42.png")
      no-repeat;
    background-size: 56%;
  }
  .swiper-button-next,
  .swiper-container-rtl .swiper-button-prev {
    right: -37px;
    left: auto;
    background: url("https://static.cmereye.com/imgs/2023/03/c1cc233620b64f31.png")
      no-repeat;
    background-size: 56%;
  }
  .swiper-button-prev,
  .swiper-button-next {
    top: 126%;
  }
  .address_box {
    display: grid;
    justify-items: start;
    grid-auto-flow: row;
    grid-template-columns: repeat(2, 1fr);
    justify-content: center;
    padding-left: 55px;
  }
  .address {
    margin-top: 10px;
    img {
      width: 22px;
      height: 32px;
    }
    p {
      margin-left: 10px;
    }
    display: flex;
    align-items: center;
  }
  .text_ev {
    h3 {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 500;
      font-size: 17px;
      line-height: 52px;
      /* or 43% */
      letter-spacing: 0.1em;
      margin-top: 10px;
      color: #4570b6;
    }
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 300;
      font-size: 17px;
      line-height: 42px;
      /* or 43% */
      color: #6d6e71;
      letter-spacing: 0.1em;
    }
  }
  .firstDiv {
    height: 346px;
    position: relative;
    background: linear-gradient(180deg, #fff 64%, #d7eaf3 0);
  }
  .swiper-slide {
    height: 171px !important;
  }
  .centerDiv {
    width: 256px;
    height: 171px !important;
    position: absolute;
    /* left: 510px; */
    top: 70px;
    left: 0;
    right: 0;
    /* display: flex; */
    /* flex-direction: column; */
    margin: auto;
    text-align: center;
  }

  .thumb-example {
    background-color: transparent;
  }

  .swiper-slide {
    background-size: cover;
    background-position: center;
  }
  .gallery-top {
    height: 80%;
    width: 100%;
  }
  .gallery-thumbs {
    height: 20%;
    box-sizing: border-box;
    padding: 10px 0;
  }
  .gallery-thumbs .swiper-slide {
    width: 37%;
    height: 57px !important;
  }
  .gallery-thumbs .swiper-slide-active {
    opacity: 1;
  }
}
</style>
