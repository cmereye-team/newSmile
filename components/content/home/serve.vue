<template>
  <div class="page_container serve-page">
    <div class="booking">
      <p>BOOKING</p>
    </div>
    <div class="pcShow flex md:justify-end flex-col items-center md:flex-row">
      <div class="serve_title">
        <p>預約服務</p>
      </div>
      <div class="serve-box serve-check" @click="serveForm2">
        <img
          src="https://static.cmereye.com/imgs/2023/03/508bd47a29791e21.jpg"
          alt=""
        />
        <p class="serve_details">術前眼睛檢查</p>
      </div>
      <div class="serve-box ml-5 yuye" @click="serveForm">
        <img
          src="https://static.cmereye.com/imgs/2023/03/c5a46c2325efaff7.jpg"
          alt=""
        />
        <p class="serve_details">講座</p>
      </div>
    </div>
    <div class="mbShow flex md:justify-end flex-col items-center md:flex-row">
      <div class="serve_title">
        <p>預約服務</p>
      </div>
      <div class="serve-box serve-check" @click="serveForm2">
        <img
          src="https://static.cmereye.com/imgs/2023/03/f25039e2bda3a90c.jpg"
          alt=""
        />
      </div>
      <div class="serve-box ml-5 yuye" @click="serveForm">
        <img
          src="https://static.cmereye.com/imgs/2023/03/6de716cfde208174.jpg "
          alt=""
        />
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
  methods: {
    serveForm2() {
      this.$router.replace("/eye-checkup");
    },
    serveForm() {
      this.$router.replace("/ophthalmicInfo/AppointForm");
    },
  },
};
</script>

<style lang="scss" scoped>
.serve-box img {
  @apply transition duration-500  ease-in-out transform  hover:scale-105 hover:-translate-x-1 hover:-translate-y-1;
}
h2 {
  font-size: 25px;
}
.serve-box {
  cursor: pointer;
  width: 580px;
  height: 100%;
  overflow: hidden;
}

.serve-page {
  position: relative;
}
@media screen and (min-width: 768px) {
  .serve-box {
    position: relative;
    .serve_details {
      position: absolute;
      bottom: 28px;
      right: 28px;
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 400;
      font-size: 30px;
      line-height: 43px;
      text-align: right;
      letter-spacing: 0.1em;

      color: #4b7bbc;
    }
  }
  .booking {
    p {
      font-family: "Baskervville" !important;
    }
    font-family: "Baskervville" !important;
    font-style: normal;
    font-weight: 400;
    font-size: 60px;
    line-height: 78px;
    display: flex;
    align-items: center;
    letter-spacing: 0.05em;
    color: rgba(174, 213, 231, 0.5);
    margin-bottom: 20px;
    margin-left: 36px;
  }
  .serve_title {
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 400;
    font-size: 43px;
    line-height: 62px;
    display: flex;
    align-items: center;
    letter-spacing: 16px;

    background: linear-gradient(177.58deg, #4b7bbc -6%, #7ed7ea 101.5%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-fill-color: transparent;
    writing-mode: tb-rl;
    position: absolute;
    top: 16px;
    left: -11px;
  }
  .more-btn {
    display: flex;
    justify-content: center;
    width: -webkit-fit-content;
    width: -moz-fit-content;
    width: fit-content;
    padding: 13px 23px;
    margin: 0 auto;
    background: linear-gradient(104.24deg, #5184c1 5.95%, #7cd3e8 114.4%);
    cursor: pointer;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 500;
      font-size: 16px;
      line-height: 20px;
      /* identical to box height, or 125% */

      letter-spacing: 0.1em;

      color: #ffffff;
    }
  }
}
@media screen and (max-width: 768px) {
  .yuye {
    bottom: -168px;
  }
  .serve-page {
    position: relative;
    height: 300px;
    margin-bottom: 50px;
  }
  .serve-box {
    position: absolute;
    width: 80%;
    right: 0;
  }
  .serve-box:nth-child(2) {
    position: absolute;
    width: 80%;
    right: 0;
    bottom: 0;
  }
  .booking {
    font-family: "Baskervville" !important;
    font-style: normal;
    font-weight: 400;
    font-size: 40px;
    line-height: 52px;
    display: flex;
    align-items: center;
    letter-spacing: 0.5em;

    color: rgba(174, 213, 231, 0.5);
    margin-bottom: 20px;
    margin-left: 56px;
  }
  .serve_title {
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 700;
    font-size: 28px;
    line-height: 41px;
    display: flex;
    align-items: center;
    letter-spacing: 0.06em;

    background: linear-gradient(177.58deg, #4b7bbc -6%, #7ed7ea 101.5%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-fill-color: transparent;
    writing-mode: tb-rl;
    position: absolute;
    top: 10px;
    left: 30px;
  }
  h2 {
    font-size: 20px;
    margin-bottom: 0px;
  }
  .serve-page {
    padding-bottom: 52px;
  }
  .more-btn {
    background: linear-gradient(104.24deg, #5184c1 5.95%, #7cd3e8 114.4%);
    width: 40%;
    margin: 0 auto;
    padding: 10px 0;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 500;
      font-size: 16px;
      line-height: 20px;
      /* identical to box height, or 125% */

      letter-spacing: 0.1em;

      color: #ffffff;
    }
  }
}
</style>
