<template>
  <div class="page_container page_box">
    <div class="booking">
      <p>COMMENTS</p>
    </div>
    <div class="aspiration">
      <div class="serve_title">
        <p>用戶心聲</p>
      </div>
      <div class="heart-box-1">
        <img
          src="https://static.cmereye.com/imgs/2023/01/7d3695d82cca797e.jpg"
          alt=""
        />
        <div class="heart-text">
          <div class="person">
            <p>姜咏鑫 Ada</p>
          </div>
          <div class="box">
            <span>每一次擘大眼都懷疑自己係咪唔記得除con既感覺</span>
          </div>
        </div>
      </div>
      <div class="heart-box-2">
        <img
          src="https://static.cmereye.com/imgs/2023/01/82809e728f70f6bc.jpg"
          alt=""
        />
        <div class="heart-text">
          <div class="box">
            <span>從未試過24hrs<br />都睇得清！</span>
          </div>
          <div class="person">
            <p>胡鴻鈞 Hubert</p>
          </div>
        </div>
      </div>
      <div class="heart-box-3">
        <img
          src="https://static.cmereye.com/imgs/2023/01/4ca3d34ccc569850.jpg"
          alt=""
        />
        <div class="heart-text">
          <div class="person">
            <p>唐浩然 Jacky</p>
          </div>
          <div class="box">
            <span>唔駛再戴con/眼鏡<br />演戲更自在！</span>
          </div>
        </div>
      </div>
      <div class="heart-box-4">
        <img
          src="https://static.cmereye.com/imgs/2023/01/bbe65cfecda34628.jpg"
          alt=""
        />
        <div class="heart-text">
          <div class="person">
            <p>陳欣妍 Shirley</p>
          </div>
          <div class="box">
            <span>以後可以戴唔會縮細我眼睛既平光鏡！</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  created() {},

  methods: {},
};
</script>
<style lang="scss" scoped>
// @tailwind base;
// @tailwind components;
// @tailwind utilities;
// // tailwind
// @layer base {
//   .heart-box-1 {
//     @apply transition duration-500  ease-in-out transform  hover:scale-105;
//   }
//   .heart-box-2 {
//     @apply transition duration-500  ease-in-out transform  hover:scale-105;
//   }
//   .heart-box-3 {
//     @apply transition duration-500  ease-in-out transform  hover:scale-105;
//   }
//   .heart-box-4 {
//     @apply transition duration-500  ease-in-out transform  hover:scale-105;
//   }
// }
.title_heart {
  h2 {
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 400;
    font-size: 25px;
    line-height: 30px;
    /* identical to box height, or 120% */

    letter-spacing: 0.1em;

    color: #444343;
  }
}
@media only screen and (min-width: 768px) {
  .page_box {
    position: relative;
  }
  .booking {
    p {
      font-family: "Baskervville" !important;
      font-style: normal;
      font-weight: 400;
      font-size: 60px !important;
      line-height: 78px;
      display: flex;
      align-items: center;
      letter-spacing: 0.05em;
      color: rgba(174, 213, 231, 0.5);
      margin-bottom: 20px;
      z-index: 66;
      margin-left: 36px;
      position: absolute;
      top: -56px;
    }
  }
  .serve_title {
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 400;
      font-size: 43px !important;
      line-height: 55px;
      display: flex;
      align-items: center;

      letter-spacing: 11px;

      background: linear-gradient(177.58deg, #4b7bbc -6%, #7ed7ea 101.5%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
      writing-mode: tb-rl;
    }

    position: absolute;

    top: -39px;

    left: -82px;
  }
  span {
    font-size: 18px !important;
  }
  p {
    font-size: 18px !important;
  }
  .title_heart {
    h2 {
      margin-top: 64px;
    }
  }
  .aspiration {
    position: relative;
    display: flex;
    position: relative;
    padding-bottom: 68px;
    margin-bottom: 5px;
    padding-top: 68px;
    margin-top: 42px;
    height: 405px;
    margin-left: 54px;
  }
  .heart-box-1 {
    position: absolute;
    bottom: 0;
    .heart-text {
      position: absolute;
      bottom: 41px;
      left: -32px;
      z-index: 10;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 15px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        padding: 10px;
        border-bottom: 1px solid #5a93c9;
        width: 194px;

        line-height: 18px;

        position: absolute;
        top: 0;
        margin-top: 28px;
        background: #fff;
        left: 28px;
        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 25px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
  .heart-box-2 {
    position: absolute;
    top: 0;
    left: 330px;
    .heart-text {
      position: absolute;
      right: -70px;
      z-index: 10;
      top: 40px;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 15px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        border-bottom: 1px solid #5a93c9;
        padding: 10px;
        width: 147px;

        line-height: 18px;

        position: absolute;
        bottom: 28px;
        background: #fff;

        left: -39px;

        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 25px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
  .heart-box-3 {
    position: absolute;
    bottom: 0;
    right: 330px;
    .heart-text {
      position: absolute;
      bottom: 41px;
      left: -32px;
      z-index: 10;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 25px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        padding: 10px;
        border-bottom: 1px solid #5a93c9;
        width: 176px;

        line-height: 18px;

        position: absolute;
        top: 0;
        margin-top: 28px;
        background: #fff;
        left: 28px;
        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 25px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
  .heart-box-4 {
    position: absolute;
    top: 0;
    right: 0px;
    .heart-text {
      position: absolute;

      z-index: 10;
      top: 87px;
      left: -67px;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 15px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        padding: 10px;
        border-bottom: 1px solid #5a93c9;
        width: 194px;

        line-height: 18px;

        position: absolute;
        bottom: 28px;
        background: #fff;
        left: -73px;
        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 25px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
}

@media only screen and (max-width: 768px) {
  .page_box {
    position: relative;
    margin-top: 100px;
  }
  .booking {
    p {
      font-family: "Baskervville" !important;
      font-style: normal;
      font-weight: 400;
      font-size: 40px !important;
      line-height: 52px;
      display: flex;
      align-items: center;
      letter-spacing: 0.05em;
      color: rgba(174, 213, 231, 0.5);
      margin-bottom: 20px;
      margin-left: 57px;
      position: absolute;
      top: -56px;
    }
  }
  .serve_title {
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 700;
      font-size: 38px !important;
      line-height: 55px;
      display: flex;
      align-items: center;

      letter-spacing: 11px;

      background: linear-gradient(177.58deg, #4b7bbc -6%, #7ed7ea 101.5%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
      writing-mode: tb-rl;
    }

    position: absolute;

    top: -34px;

    left: 0px;
  }
  .aspiration {
    display: flex;
    position: relative;
    padding-bottom: 68px;
    margin-bottom: 68px;
    height: 308vw;
    flex-direction: column;
  }
  .heart-box-1 {
    position: absolute;
    right: 0;
    .heart-text {
      position: absolute;
      bottom: 41px;
      left: -32px;
      z-index: 10;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 15px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        padding: 6px;
        border-bottom: 1px solid #5a93c9;
        width: 160px;
        position: absolute;
        top: 25px;
        background: #fff;
        left: 28px;
        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 15px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
  .heart-box-2 {
    position: absolute;
    top: 85vw;
    left: 0;
    .heart-text {
      position: absolute;
      right: -70px;
      z-index: 10;
      top: 40px;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 15px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        padding: 6px;
        border-bottom: 1px solid #5a93c9;
        width: 123px;
        position: absolute;
        top: -57px;
        background: #fff;
        left: -51px;
        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 15px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
  .heart-box-3 {
    position: absolute;
    top: 164vw;
    right: 0px;
    left: 0;
    display: flex;
    justify-content: center;
    .heart-text {
      position: absolute;
      bottom: 41px;
      left: 17px;
      z-index: 10;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 15px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        padding: 6px;
        border-bottom: 1px solid #5a93c9;
        width: 160px;
        position: absolute;
        top: 25px;
        background: #fff;
        left: 28px;
        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 15px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
  .heart-box-4 {
    position: absolute;
    bottom: 0;
    right: 0px;
    .heart-text {
      position: absolute;

      z-index: 10;
      top: 87px;
      left: -37px;
      .person {
        z-index: 10;
      }
      p {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 12px;
        line-height: 15px;
        text-align: center;
        letter-spacing: 0.06em;

        color: #ffffff;
        background: linear-gradient(91.62deg, #5992c8 6.27%, #81dbec 99.02%);
        width: max-content;
        padding: 7px;
      }
      .box {
        padding: 6px;
        border-bottom: 1px solid #5a93c9;
        width: 132px;
        position: absolute;
        top: -54px;
        background: #fff;
        left: -51px;
        z-index: -1;
        span {
          font-family: "Inter";
          font-style: normal;
          font-weight: 300;
          font-size: 12px;
          line-height: 15px;
          text-align: center;
          letter-spacing: 0.06em;

          color: #6d6e71;
        }
      }
    }
  }
}
</style>
