<template>
  <div class="page_container">
    <div class="flex justify-center md:mt-28 mt-10">
      <h2>矯視前停 con 知多啲</h2>
    </div>
    <div>
      <div class="flex justify-center pcShow">
        <img
          src="https://static.cmereye.com/imgs/2022/12/af21e2a1ef419d29.jpg"
          alt=""
        />
      </div>
      <div class="flex preorth_box">
        <div class="preorth flex justify-evenly flex-col justify-center">
          <img
            src="https://static.cmereye.com/imgs/2022/12/c07c6b4f21d225d5.png"
            alt=""
          />
          <span class="pt-3">前台登記及<br class="pcShow" />初步眼睛檢查</span>
        </div>
        <div class="flex flex-col justify-center mt-1 mx-5 arrow">
          <img
            src="https://static.cmereye.com/imgs/2022/12/5dc8f0ff1a0bb90d.png"
            alt=""
          />
        </div>
        <div class="preorth flex justify-evenly flex-col justify-center">
          <img
            src="https://static.cmereye.com/imgs/2022/12/7b3798d7b61abfb9.png"
            alt=""
          />
          <span class="pt-3">詳細屈光檢查</span>
        </div>
        <div class="flex flex-col justify-center mt-1 mx-5 arrow">
          <img
            src="https://static.cmereye.com/imgs/2022/12/5dc8f0ff1a0bb90d.png"
            alt=""
          />
        </div>
        <div class="preorth flex justify-evenly flex-col justify-center">
          <img
            src="https://static.cmereye.com/imgs/2022/12/2f2d444c97114450.png"
            alt=""
          />
          <span class="pt-3">散曈</span>
        </div>
        <div class="flex flex-col justify-center mt-1 mx-5 arrow">
          <img
            src="https://static.cmereye.com/imgs/2022/12/5dc8f0ff1a0bb90d.png"
            alt=""
          />
        </div>
        <div class="preorth flex justify-evenly flex-col justify-center">
          <img
            src="https://static.cmereye.com/imgs/2022/12/032341e288d255ad.png"
            alt=""
          />
          <span class="pt-3">全面眼底檢查</span>
        </div>
        <div class="arrow-two">
          <div class="Inappropriate">
            <div class="flex flex-col justify-center mt-1 mx-5 arrow-top">
              <img
                src="https://static.cmereye.com/imgs/2022/12/5dc8f0ff1a0bb90d.png"
                alt=""
              />
            </div>
            <div class="Inappropriate-box">
              <span>不合適</span>
              <p>應盡快接受相關治療</p>
            </div>
          </div>
          <div class="appropriate">
            <div class="flex flex-col justify-center mt-1 mx-5 arrow-botom">
              <img
                src="https://static.cmereye.com/imgs/2022/12/5dc8f0ff1a0bb90d.png"
                alt=""
              />
            </div>
            <div class="appropriate-box">
              <span>合適</span>
              <p>預約第二次檢查及<br />同日矯視</p>
            </div>
          </div>
        </div>
      </div>
      <div class="flex flex-col mb-10 beizhu">
        <p>備註：</p>
        <p>1. 基本檢查包括：屈光檢查、電腦驗光、眼壓、角膜厚度等</p>
        <p>
          2.
          詳細眼底檢查包括：淚水分泌測試、瞳孔測量、角膜地形掃描及像差、雙眼內皮細胞分析、散瞳眼底檢查、光學相干斷層掃描(如需要)、<br />掃描激光眼底檢查(如需要)
        </p>
        <p>3. 散瞳/ 放大瞳孔後：</p>
        <p>·觀看近物時視野變得模糊</p>
        <p>·有輕微畏光情況，可帶備太陽眼鏡</p>
        <p>·切勿駕駛</p>
        <p>·請帶備太陽眼鏡</p>
        <p>·放大瞳孔的效果一般會在4至6小時後消失</p>
      </div>
      <div class="flex justify-center">
        <a href="#" class="mbShow">
          <button>
            <div class="flex btn-yuyue">
              <img
                src="https://static.cmereye.com/imgs/2022/12/f3fcc54f4a9b0108.png"
                alt=""
                style="width: 12vw"
              />
              <div class="flex flex-col justify-center" style="padding: 0 10px">
                <span>立即預約 / 查詢</span>
                <span>6061 0511</span>
              </div>
            </div>
          </button>
        </a>
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
h2 {
  font-size: 25px;
}
@media screen and (min-width: 768px) {
  .beizhu {
    margin-bottom: 85px;
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 300;
      font-size: 18px;
      line-height: 30px;
      /* or 200% */

      letter-spacing: 0.1em;

      color: #000000;
    }
  }

  .preorth_box {
    display: flex;
    justify-content: space-evenly;
    margin: 100px 0;
    .preorth {
      justify-content: flex-end;
      img {
        width: 94px;
        margin: auto;
      }
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 300;
        font-size: 18px;
        line-height: 30px;
        /* or 200% */

        letter-spacing: 0.1em;

        color: #000000;
      }
    }
    .preorth:nth-child(5) img {
      margin-bottom: 10px;
      width: 45px;
      margin: auto;
    }
    .preorth:nth-child(7) img {
      margin-bottom: 42px;
    }
  }
  .arrow-two {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    .arrow-top {
      img {
        transform: rotate(-45deg);
      }
    }
    .arrow-botom {
      transform: rotateX(180deg) rotate(-45deg);
    }
  }
  .Inappropriate {
    display: flex;
    margin: 15px 0;
    .Inappropriate-box {
      width: 186px;
      background-color: #fff2f2;
      padding: 10px;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 700;
        font-size: 18px;
        line-height: 20px;
        /* identical to box height, or 111% */

        letter-spacing: 0.1em;

        background: linear-gradient(92.06deg, #558bc6 7.92%, #78cbe4 79.85%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        text-fill-color: transparent;
      }
      p {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 300;
        font-size: 16px;
        line-height: 20px;
        /* or 125% */

        letter-spacing: 0.1em;

        color: #000000;
      }
    }
  }
  .appropriate {
    display: flex;
    margin: 15px 0;
    .appropriate-box {
      background-color: #eefbf2;
      padding: 10px;
      width: 186px;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 700;
        font-size: 18px;
        line-height: 20px;
        /* identical to box height, or 111% */

        letter-spacing: 0.1em;

        background: linear-gradient(92.06deg, #558bc6 7.92%, #78cbe4 79.85%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        text-fill-color: transparent;
      }
      p {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 300;
        font-size: 16px;
        line-height: 20px;
        /* or 125% */

        letter-spacing: 0.1em;

        color: #000000;
      }
    }
  }
}
@media screen and (max-width: 768px) {
  h2 {
    font-size: 16px;
  }
  .btn-yuyue {
    margin-bottom: 10vw;
  }
  .Inappropriate-box {
    // width: 186px;
    background-color: #fff2f2;
    padding: 10px;
    width: 70%;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 700;
      font-size: 18px;
      line-height: 20px;
      /* identical to box height, or 111% */

      letter-spacing: 0.1em;

      background: linear-gradient(92.06deg, #558bc6 7.92%, #78cbe4 79.85%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
    }
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 300;
      font-size: 16px;
      line-height: 20px;
      /* or 125% */

      letter-spacing: 0.1em;

      color: #000000;
    }
  }

  .appropriate-box {
    background-color: #eefbf2;
    padding: 10px;
    // width: 186px;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 700;
      font-size: 18px;
      line-height: 20px;
      /* identical to box height, or 111% */

      letter-spacing: 0.1em;

      background: linear-gradient(92.06deg, #558bc6 7.92%, #78cbe4 79.85%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
    }
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 300;
      font-size: 16px;
      line-height: 20px;
      /* or 125% */

      letter-spacing: 0.1em;

      color: #000000;
    }
  }
  .arrow-two {
    display: flex;
    .arrow-top {
      transform: rotateY(180deg) rotate(45deg);
      padding: 30px 10px;
      img {
        max-width: 20vw;
      }
    }
    .arrow-botom {
      transform: rotate(45deg);
      padding: 30px 10px;
      img {
        max-width: 20vw;
      }
    }
  }
  .preorth_box {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 40px;
    img {
      max-width: 100%;
    }
    .preorth {
      display: flex;
      align-items: center;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 300;
        font-size: 16px;
        line-height: 20px;
        /* or 125% */

        text-align: center;
        letter-spacing: 0.1em;

        color: #000000;
      }
    }
  }
  .arrow {
    padding: 40px 0;
    transform: rotate(90deg);
  }
}
</style>
