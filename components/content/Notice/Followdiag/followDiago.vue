<template>
  <div class="page_container">
    <div class="flex justify-center md:mt-28 mt-10">
      <h2>矯視後覆診</h2>
    </div>
    <div class="time-box">
      <div class="one">
        <div class="piont"></div>
        <span>翌日</span>
      </div>
      <div class="two">
        <div class="piont"></div>
        <span>一星期</span>
      </div>
      <div class="three">
        <div class="piont"></div>
        <span>一個月</span>
      </div>
      <div class="four">
        <div class="piont"></div>
        <div class="arrow"></div>
        <span>三個月</span>
      </div>
      <div class="five">
        <div class="piont"></div>

        <span
          >六個月<br />
          （或按醫生之需要覆診指示）</span
        >
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
  .five {
    display: flex;
    flex-direction: column;
    align-items: center;

    .piont {
      background: #4b7bbc;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 20px;
      border-style: solid;
    }
  }
  .four {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    .piont {
      background: #62a5d1;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 20px;
    }
    .arrow {
      background: linear-gradient(229.22deg, #4e81bf 6.93%, #62a5d1 93.07%);
      content: "";
      display: inline-block;
      height: 3px;
      left: 14px;
      position: absolute;
      top: 13px;
      bottom: 0;
      display: flex;
      text-align: center;
      width: 192px;
    }
    .arrow::after {
      content: "";
      position: absolute;
      bottom: -8px;
      right: 0px;
      border-color: #4b7bbc;
      border-style: solid;
      border-width: 3px 3px 0 0;
      transform: rotate(45deg);
      width: 20px;
      height: 20px;
      background-color: transparent;
    }
    // .piont::after {
    //   background: linear-gradient(229.22deg, #4e81bf 6.93%, #62a5d1 93.07%);
    //   content: "";
    //   display: inline-block;
    //   height: 3px;
    //   left: 14px;
    //   position: absolute;
    //   top: 13px;
    //   bottom: 0;
    //   display: flex;
    //   text-align: center;
    //   width: 192px;
    // }
  }
  .three {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    .piont {
      background: #62a5d1;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 20px;
    }
    .piont::after {
      background: linear-gradient(229.22deg, #4e81bf 6.93%, #62a5d1 93.07%);
      content: "";
      display: inline-block;
      height: 3px;
      left: 14px;
      position: absolute;
      top: 13px;
      bottom: 0;
      display: flex;
      text-align: center;
      width: 192px;
    }
  }
  .two {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    .piont {
      background: #7ed7ea;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 20px;
    }
    .piont::after {
      background: linear-gradient(229.22deg, #62a5d1 6.93%, #7ed7ea 93.07%);
      content: "";
      display: inline-block;
      height: 3px;
      left: 14px;
      position: absolute;
      top: 13px;
      bottom: 0;
      display: flex;
      text-align: center;
      width: 192px;
    }
  }
  .one {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    .piont {
      background: #7ed7ea;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 20px;
    }
    .piont::after {
      background: linear-gradient(229.22deg, #7ed7ea 6.93%, #7ed7ea 93.07%);
      content: "";
      display: inline-block;
      height: 3px;
      left: 14px;
      position: absolute;
      top: 13px;
      bottom: 0;
      width: 172px;
      display: flex;
      text-align: center;
    }
  }

  .time-box {
    display: flex;
    justify-content: space-evenly;
    text-align: center;
  }
}
@media screen and (max-width: 768px) {
  h2 {
    font-size: 16px;
  }
  .five {
    display: flex;
    flex-direction: column;
    align-items: center;

    .piont {
      background: #4b7bbc;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 5px;
      border-style: solid;
    }
  }
  .four {
    margin-bottom: 96px;
    display: flex;
    position: relative;

    flex-direction: column;
    align-items: center;
    .piont {
      background: #62a5d1;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 5px;
    }
    span {
      position: absolute;
      margin-right: 92px;
    }
    .arrow {
      background: linear-gradient(229.22deg, #4e81bf 6.93%, #62a5d1 93.07%);
      content: "";
      display: inline-block;
      height: 3px;
      position: absolute;
      width: 86px;
      transform: matrix(0, 1, 1, 0, 0, 0);
      top: 53px;
    }
    .arrow::after {
      content: "";
      position: absolute;
      bottom: -8px;
      right: 0px;
      border-color: #4b7bbc;
      border-style: solid;
      border-width: 3px 3px 0 0;
      transform: rotate(45deg);
      width: 20px;
      height: 20px;
      background-color: transparent;
    }
    // .piont::after {
    //   background: linear-gradient(229.22deg, #4e81bf 6.93%, #62a5d1 93.07%);
    //   content: "";
    //   display: inline-block;
    //   height: 3px;
    //   left: 14px;
    //   position: absolute;
    //   top: 13px;
    //   bottom: 0;
    //   display: flex;
    //   text-align: center;
    //   width: 192px;
    // }
  }
  .three {
    margin-bottom: 96px;
    display: flex;
    flex-direction: column;
    align-items: center;
    span {
      position: absolute;
      margin-left: 92px;
    }
    .piont {
      background: #62a5d1;
      position: relative;

      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 5px;
    }
    .piont::after {
      background: linear-gradient(229.22deg, #4e81bf 6.93%, #62a5d1 93.07%);

      content: "";
      display: inline-block;
      height: 3px;
      position: absolute;
      width: 152px;
      transform: matrix(0, 1, 1, 0, 0, 0);
      left: -61px;
      top: 78px;
    }
  }
  .two {
    margin-bottom: 96px;
    display: flex;
    flex-direction: column;
    align-items: center;
    span {
      position: absolute;
      margin-right: 92px;
    }
    .piont {
      position: relative;
      background: #7ed7ea;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 5px;
    }
    .piont::after {
      background: linear-gradient(229.22deg, #62a5d1 6.93%, #7ed7ea 93.07%);
      content: "";
      display: inline-block;
      height: 3px;
      position: absolute;
      width: 152px;
      transform: matrix(0, 1, 1, 0, 0, 0);
      left: -61px;
      top: 78px;
    }
  }
  .one {
    margin-bottom: 96px;

    display: flex;
    flex-direction: column;
    align-items: center;
    .piont {
      position: relative;
      background: #7ed7ea;
      width: 29px;
      height: 29px;
      border-radius: 50%;
      margin-bottom: 5px;
    }
    span {
      position: absolute;
      margin-left: 92px;
    }
    .piont::after {
      background: linear-gradient(229.22deg, #7ed7ea 6.93%, #7ed7ea 93.07%);
      content: "";
      display: inline-block;
      height: 3px;
      position: absolute;
      width: 116px;
      transform: matrix(0, 1, 1, 0, 0, 0);
      left: -43px;
      top: 79px;
    }
  }

  .time-box {
    display: flex;
    text-align: center;
    flex-direction: column;
  }
}
</style>
