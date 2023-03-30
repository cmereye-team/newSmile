<template>
  <div class="section flex justify-start items-center">
    <div class="des_box">
      <h3 class="gradient_font">
        <slot name="title"></slot>
      </h3>
      <p>
        <slot name="des"></slot>
      </p>
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
@media screen and (min-width: 768px) {
  .section {
    height: 480px;
    background-size: cover !important;
    background-repeat: no-repeat;
    padding-left: 63px;
    .des_box {
      width: 648px;

      margin-bottom: 75px;

      h3 {
        font-weight: 700;
        font-size: 28px;
      }
      p {
        font-family: "Noto Sans JP";
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 30px;
        /* or 200% */
        margin-top: 12px;
        letter-spacing: 0.1em;
        text-align: justify;
        color: #9b9b9b;
      }
    }
  }
}
@media screen and (max-width: 768px) {
  .section {
    height: 76vw;
  }
  .des_box {
    padding-left: 28px;
    h3 {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 800;
      font-size: 17px;
      line-height: 15px;
      /* or 125% */

      letter-spacing: 0.1em;

      background: linear-gradient(90.24deg, #4570b6 12.21%, #81dbec 87.2%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
    }
    span {
      font-size: 11px;
    }
    p {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 400;
      font-size: 10px;
      line-height: 18px;
      letter-spacing: 0.08em;
      color: #9b9b9b;
      width: 55vw;
      padding-top: 18px;
    }
  }
}
</style>
