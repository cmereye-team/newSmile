<template>
  <div class="tab flex justify-center page_container flex-col" id="tab">
    <div class="flex justify-center">
      <h2>收費詳情</h2>
    </div>

    <div class="tab-control">
      <div
        class="tab-control-item"
        v-for="(item, index) in title"
        :key="item"
        :class="{ active: action === index }"
        @click="titelclick(index)"
      >
        <span>{{ item }}</span>
        <hr class="mbShow" />
      </div>
    </div>
    <div v-if="currentTitleIndex === 0" class="flex flex-col items-center">
      <div class="md:mt-10" id="smile"><h2 style="margin-bottom: 0 !important;">Smile 微笑矯視</h2></div>
      <div class="table-1-box">
        <table summary="本診所價目清晰，絕無其他額外收費" class="gdp">
          <caption>
            本診所價目清晰，絕無其他額外收費
          </caption>
          <thead>
            <tr>
              <th><p>單眼</p></th>
              <th><p>雙眼</p></th>
            </tr>
          </thead>

          <tbody>
            <tr>
              <td><span>$15,000</span></td>
              <td><span>$29,000</span></td>
            </tr>
            <tr>
              <td colspan="4" id="blue">優惠（即日至30.4.2023）</td>
            </tr>
            <tr>
              <td><span>$12,500*</span></td>
              <td><span>$20,000*</span></td>
            </tr>
            <tr>
              <td colspan="4" class="free">術前檢查費用 $100^</td>
            </tr>
          </tbody>
        </table>
        <span>*指定信用卡（東亞/渣打/滙豐）可享6/12個月免息分期</span><br />
        <span>^完成矯視後可退回術前檢查費用</span>
      </div>
      <div class="pb-20 taoc_boxs">
        <div class="md:mt-20 mt-10 taoc_box">
          <div class="titel">
            <span>套餐包括</span>
          </div>
          <div class="icon-box">
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/1ec75abea01070d2.png"
                alt=""
              />
              <span>眼科專科醫生檢查</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/c0f749ea1b2c488f.png"
                alt=""
              />
              <span>術前檢查費用</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/aa210b095705a9b2.png"
                alt=""
              />
              <span>術後3次覆診<i style="font-size: 14px;">#</i> </span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/1cfef0fbde2b4cdb.png"
                alt=""
              />
              <span>增進手術<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/523fa3d1f9f21b0b.png"
                alt=""
              />
              <span>無限視光檢查<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/68d11f0b9181e1a4.png"
                alt=""
              />
              <span>手術當日藥費</span>
            </div>
          </div>
        </div>
        <span
          >#需要術後一年內完成。如超過一年，需另作預約，診金按正常（非矯視套餐）收費</span
        >
      </div>
       <div class="md:mt-10" id="ICL"><h2 style="margin-bottom: 0 !important;">ICL植入式隱形眼鏡</h2></div>
      <div class="table-1-box pcShow">
        <table summary="本診所價目清晰，絕無其他額外收費" class="gdp">
          <caption>
            本診所價目清晰，絕無其他額外收費
          </caption>
          <thead>
            <tr>
              <th><p>單眼 (不帶散光)</p></th>
              <th><p>單眼 (帶散光)</p></th>
              <th><p>雙眼 (不帶散光)</p></th>
              <th><p>雙眼 (帶散光)</p></th>
            </tr>
          </thead>

          <tbody>
            <tr>
              <td><span>$45,000</span></td>
              <td><span>$50,000</span></td>
              <td><span>$85,000</span></td>
              <td><span>$95,000</span></td>
            </tr>
            <tr>
              <td colspan="4" id="blue">優惠（即日至30.4.2023）</td>
            </tr>
            <tr>
              <td><span>$38,000*</span></td>
              <td><span>$42,000*</span></td>
              <td><span>$67,000*</span></td>
              <td><span>$72,000*</span></td>
            </tr>
            <tr>
              <td colspan="4" class="free">術前檢查費用 $500^</td>
            </tr>
          </tbody>
        </table>
        <span>*指定信用卡（東亞/渣打/滙豐）可享6/12個月免息分期</span><br />
        <span>^完成矯視後可退回術前檢查費用</span>
      </div>
      <div class="table-1-box mbShow">
        <table summary="本診所價目清晰，絕無其他額外收費" class="gdp">
          <caption>
            本診所價目清晰，絕無其他額外收費
          </caption>
          <thead>
            <tr>
              <th><p>單眼</p></th>
              <th><p>雙眼</p></th>
            </tr>
          </thead>

          <tbody>
            <tr>
              <td><span>$15,000</span></td>
              <td><span>$29,000</span></td>
            </tr>
            <tr>
              <td colspan="4" id="blue">優惠（即日至30.4.2023）</td>
            </tr>
            <tr>
              <td><span>$12,500*</span></td>
              <td><span>$20,000*</span></td>
            </tr>
            <tr>
              <td colspan="4" class="free">術前檢查費用 $100^</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="table-1-box mbShow">
        <table summary="本診所價目清晰，絕無其他額外收費" class="gdp">
          <thead>
            <tr>
              <th><p>單眼</p></th>
              <th><p>雙眼</p></th>
            </tr>
          </thead>

          <tbody>
            <tr>
              <td><span>$15,000</span></td>
              <td><span>$29,000</span></td>
            </tr>
            <tr>
              <td colspan="4" id="blue">優惠（即日至30.4.2023）</td>
            </tr>
            <tr>
              <td><span>$12,500*</span></td>
              <td><span>$20,000*</span></td>
            </tr>
            <tr>
              <td colspan="4" class="free">術前檢查費用 $100^</td>
            </tr>
          </tbody>
        </table>
        <span>*指定信用卡（東亞/渣打/滙豐）可享6/12/18/24個月免息分期</span><br />
        <span>*完成矯視後可退回術前檢查費用</span>
      </div>
      <div class="pb-20 taoc_boxs">
        <div class="mt-20 taoc_box taoc_box_2">
          <div class="titel">
            <span>套餐包括</span>
          </div>
          <div class="icon-box">
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/1ec75abea01070d2.png"
                alt=""
              />
              <span>眼科專科醫生檢查</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/c0f749ea1b2c488f.png"
                alt=""
              />
              <span>術前檢查費用 </br>（藥費另外收費）</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/aa210b095705a9b2.png"
                alt=""
              />
              <span>術後3次覆診<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/523fa3d1f9f21b0b.png"
                alt=""
              />
              <span>無限視光檢查<i style="font-size: 14px;">#</i></span>
            </div>
          </div>
        </div>
        <span class="shoufei"
          >#需要術後一年內完成。如超過一年，需另作預約，診金按正常（非矯視套餐）收費</span
        >
      </div>

      <div class="md:mt-10" id="LASIK"><h2 style="margin-bottom: 0 !important;">LASIK 激光矯視</h2></div>
       <div class="table-1-box">
        <table summary="本診所價目清晰，絕無其他額外收費" class="gdp">
          <caption>
            本診所價目清晰，絕無其他額外收費
          </caption>
          <thead>
            <tr>
              <th><p>單眼</p></th>
              <th><p>雙眼</p></th>
            </tr>
          </thead>

          <tbody>
            <tr>
              <td><span>$15,000</span></td>
              <td><span>$29,000</span></td>
            </tr>
            <tr>
              <td colspan="4" id="blue">優惠（即日至30.4.2023）</td>
            </tr>
            <tr>
              <td><span>$12,500*</span></td>
              <td><span>$20,000*</span></td>
            </tr>
            <tr>
              <td colspan="4" class="free">術前檢查費用 $100^</td>
            </tr>
          </tbody>
        </table>
        <span>*指定信用卡（東亞/渣打/滙豐）可享6/12個月免息分期</span><br />
        <span>^完成矯視後可退回術前檢查費用</span>
      </div>
      <div class="pb-20 taoc_boxs">
        <div class="md:mt-20 mt-10 taoc_box">
          <div class="titel">
            <span>套餐包括</span>
          </div>
          <div class="icon-box">
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/1ec75abea01070d2.png"
                alt=""
              />
              <span>眼科專科醫生檢查</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/c0f749ea1b2c488f.png"
                alt=""
              />
              <span>術前檢查費用</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/aa210b095705a9b2.png"
                alt=""
              />
              <span>術後3次覆診<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/1cfef0fbde2b4cdb.png"
                alt=""
              />
              <span>增進手術<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/523fa3d1f9f21b0b.png"
                alt=""
              />
              <span>無限視光檢查<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/68d11f0b9181e1a4.png"
                alt=""
              />
              <span>手術當日藥費</span>
            </div>
          </div>
        </div>
        <span
          >#需要術後一年內完成。如超過一年，需另作預約，診金按正常（非矯視套餐）收費</span
        >
      </div>

      <div class="md:mt-10" id="Clear-Vision"><h2 style="margin-bottom: 0 !important;">Clear-Vision  激光矯視</h2></div>
      <div class="table-box_four pcShow">
<table  summary="本診所價目清晰，絕無其他額外收費" class="gdp">
        <caption >
            本診所價目清晰，絕無其他額外收費
          </caption>
        <colgroup>
          <col width="70" style="width: 50pt" />
          <col width="140" style="width: 105pt" />
          <col width="72" style="width: 54pt" span="6" />
        </colgroup>
        <tbody>
          <tr height="19">
            <td class="boder-none"></td>
            <td rowspan="2" class="et2 table-head-blue"><span>單焦點人工晶體 <br>(不帶散光)</span></td>
            <td colspan="2" rowspan="2" class="et2 table-head-blue-2"><span>單焦點人工晶體 <br>(散光)</span></td>
            <td colspan="2" rowspan="2" class="et2 table-head-blue">
              <span>多焦點人工晶體<br>(不帶散光)</span>
            </td>
            <td colspan="2" rowspan="2" class="et2 table-head-blue-2"><span>多焦點人工晶體<br> (散光)</span></td>
          </tr>
          <tr height="10">
            <!-- <td class="boder-none"></td> -->
          </tr>
          <tr height="19" class="jiage">
            <td class="danyan" style="width: 73px !important;"><span class="text">單眼</span></td>
            <td class><span>$18,000 - $35,000</span></td>
            <td colspan="2" class="et4"><span>$23,000 - $41,000</span></td>
            <td colspan="2" class="et4"><span>$26,000 - $51,000</span></td>
            <td colspan="2" class="et4"><span>$31,000 - $51,000</span></td>
          </tr>
          <tr height="19" class="free">
            <td class="boder-none"></td>
            <td colspan="7" class="et2"><span>術前檢查費用 $600</span></td>
          </tr>
        </tbody>
      </table>
      </div>
     <div class="table-1-box mbShow">
        <table  class="gdp">
           <caption>
            本診所價目清晰，絕無其他額外收費
          </caption>
          <thead>
            <tr>
              <th style="padding: 12px 0;"><p>單焦點人工晶體 <br>(不帶散光)</p></th>
              <th style="padding: 12px 0;"><p>單焦點人工晶體<br> (帶散光)</p></th>
            </tr>
          </thead>

          <tbody>
            <tr >
              <td>
                <div  class="my-5">
              <span>$18,000 </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $35,000</span>
                </div></td>
              <td> <div  class="my-5">
              <span>$23,000  </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $41,000</span>
                </div></td>
            </tr>
            <tr>
                <th style="border-radius: 0 !important;padding: 12px 0;"><p>多焦點人工晶體 <br>(不帶散光)</p></th>
              <th style="border-radius: 0 !important; padding: 12px 0;"><p>多焦點人工晶體 <br>(帶散光)</p></th>
            </tr>
           <tr >
              <td>
                <div  class="my-5">
              <span>$26,000 </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $51,000</span>
                </div></td>
              <td> <div  class="my-5">
              <span>$31,000  </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $51,000</span>
                </div></td>
            </tr>
            <tr>
              <td colspan="4" class="free" style="padding: 10px 0;">術前檢查費用 $600</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
    <div v-else-if="currentTitleIndex === 1" class="flex flex-col items-center">
      
    </div>
    <div v-else-if="currentTitleIndex === 2" class="flex flex-col items-center">
      <div class="table-1-box">
        <table summary="本診所價目清晰，絕無其他額外收費" class="gdp">
          <caption>
            本診所價目清晰，絕無其他額外收費
          </caption>
          <thead>
            <tr>
              <th><p>單眼</p></th>
              <th><p>雙眼</p></th>
            </tr>
          </thead>

          <tbody>
            <tr>
              <td><span>$15,000</span></td>
              <td><span>$29,000</span></td>
            </tr>
            <tr>
              <td colspan="4" id="blue">優惠（即日至30.4.2023）</td>
            </tr>
            <tr>
              <td><span>$12,500*</span></td>
              <td><span>$20,000*</span></td>
            </tr>
            <tr>
              <td colspan="4" class="free">術前檢查費用 $100^</td>
            </tr>
          </tbody>
        </table>
        <span>*指定信用卡（東亞/渣打/滙豐）可享6/12個月免息分期</span><br />
        <span>^完成矯視後可退回術前檢查費用</span>
      </div>
      <div class="pb-20">
        <div class="md:mt-20 mt-10 taoc_box">
          <div class="titel">
            <span>套餐包括</span>
          </div>
          <div class="icon-box">
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/1ec75abea01070d2.png"
                alt=""
              />
              <span>眼科專科醫生檢查</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/c0f749ea1b2c488f.png"
                alt=""
              />
              <span>術前檢查費用</span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/aa210b095705a9b2.png"
                alt=""
              />
              <span>術後3次覆診<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/1cfef0fbde2b4cdb.png"
                alt=""
              />
              <span>增進手術<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/523fa3d1f9f21b0b.png"
                alt=""
              />
              <span>無限視光檢查<i style="font-size: 14px;">#</i></span>
            </div>
            <div class="box">
              <img
                src="https://static.cmereye.com/imgs/2023/01/68d11f0b9181e1a4.png"
                alt=""
              />
              <span>手術當日藥費</span>
            </div>
          </div>
        </div>
        <span
          >#需要術後一年內完成。如超過一年，需另作預約，診金按正常（非矯視套餐）收費</span
        >
      </div>
    </div>
    <div v-else class="flex flex-col items-center">
      <div class="table-box_four pcShow">
<table  summary="本診所價目清晰，絕無其他額外收費" class="gdp">
        <caption >
            本診所價目清晰，絕無其他額外收費
          </caption>
        <colgroup>
          <col width="70" style="width: 50pt" />
          <col width="140" style="width: 105pt" />
          <col width="72" style="width: 54pt" span="6" />
        </colgroup>
        <tbody>
          <tr height="19">
            <td class="boder-none"></td>
            <td rowspan="2" class="et2 table-head-blue"><span>單焦點人工晶體 <br>(不帶散光)</span></td>
            <td colspan="2" rowspan="2" class="et2 table-head-blue-2"><span>單焦點人工晶體 <br>(散光)</span></td>
            <td colspan="2" rowspan="2" class="et2 table-head-blue">
              <span>多焦點人工晶體<br>(不帶散光)</span>
            </td>
            <td colspan="2" rowspan="2" class="et2 table-head-blue-2"><span>多焦點人工晶體<br> (散光)</span></td>
          </tr>
          <tr height="10">
            <!-- <td class="boder-none"></td> -->
          </tr>
          <tr height="19" class="jiage">
            <td class="danyan" style="width: 73px !important;"><span class="text">單眼</span></td>
            <td class><span>$18,000 - $35,000</span></td>
            <td colspan="2" class="et4"><span>$23,000 - $41,000</span></td>
            <td colspan="2" class="et4"><span>$26,000 - $51,000</span></td>
            <td colspan="2" class="et4"><span>$31,000 - $51,000</span></td>
          </tr>
          <tr height="19" class="free">
            <td class="boder-none"></td>
            <td colspan="7" class="et2"><span>術前檢查費用 $600</span></td>
          </tr>
        </tbody>
      </table>
      </div>
     <div class="table-1-box mbShow">
        <table  class="gdp">
           <caption>
            本診所價目清晰，絕無其他額外收費
          </caption>
          <thead>
            <tr>
              <th style="padding: 12px 0;"><p>單焦點人工晶體 <br>(不帶散光)</p></th>
              <th style="padding: 12px 0;"><p>單焦點人工晶體<br> (帶散光)</p></th>
            </tr>
          </thead>

          <tbody>
            <tr >
              <td>
                <div  class="my-5">
              <span>$18,000 </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $35,000</span>
                </div></td>
              <td> <div  class="my-5">
              <span>$23,000  </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $41,000</span>
                </div></td>
            </tr>
            <tr>
                <th style="border-radius: 0 !important;padding: 12px 0;"><p>多焦點人工晶體 <br>(不帶散光)</p></th>
              <th style="border-radius: 0 !important; padding: 12px 0;"><p>多焦點人工晶體 <br>(帶散光)</p></th>
            </tr>
           <tr >
              <td>
                <div  class="my-5">
              <span>$26,000 </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $51,000</span>
                </div></td>
              <td> <div  class="my-5">
              <span>$31,000  </span>
              <div style="margin:10px 0">
                <span >｜</span>
              </div>
             <span> $51,000</span>
                </div></td>
            </tr>
            <tr>
              <td colspan="4" class="free" style="padding: 10px 0;">術前檢查費用 $600</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      activeNames: ["1"],
      action:0,
      currentTitleIndex: 0,
      title: [
        "Smile 微笑矯視",
        "ICL植入式隱形眼鏡",
        "LASIK 激光矯視",
        "Clear-Vision",
      ],
      list: [
        {
          id: 1,
          title: "收費詳情",
        },
        {
          id: 2,
          title: "消費券詳情",
        },
      ],
      currentIndex: 1, // 当前点击的tab的索引
    };
  },
  created() {},
  methods: {
    titelclick(index) {
      this.action = index
      if(index === 0){
        window.location.href='/charge-detail#smile'
      }else if(index === 1){
  window.location.href='/charge-detail#ICL'
      }else if(index === 2){
  window.location.href='/charge-detail#LASIK'
      }else{  window.location.href='/charge-detail#Clear-Vision'

      }
    },
    //判断是否打开
    judgeActive(data) {
      console.log(data);
      return this.activeNames.indexOf(data);
    },
    handleChange(val) {
      console.log(val);
    },
    exchangeTab(index) {
      // 点击tab切换
      this.currentIndex = index;
      // console.log(index);
    },
  },
};
</script>
<style lang="scss" scoped>
.contents {
  display: flex;
}
h2 {
  font-size: 25px;
}
span {
  font-size: 14px;
}

ul {
  margin: 0;
  padding: 0;
  height: 50px;
  position: absolute;
}
li {
  cursor: pointer;
  box-sizing: border-box;
  list-style: none;
  text-align: center;
  line-height: 50px;
  float: left;
  border-bottom: 2px solid #ddd;
  // border-bottom: 2px solid linear-gradient(#81dbec,#4570b6 );
  border-image: -webkit-linear-gradient(60deg, #81dbec, #4570b6) 1 2;
  margin: 0 5vw;
  width: 30vw;
}
p {
  font-weight: 800;
  font-size: 18px;
  background-image: -webkit-linear-gradient(bottom, #81dbec, #4570b6);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.active {
  background-color: #f3fcfe;
  display: block;
}

.tables {
  margin-top: 12vw;
}
.gdp {
  margin-bottom: 0px;
}
.gdp caption {
  font-family: "Noto Sans HK";
  font-style: normal;
  font-weight: 350;
  font-size: 13px;
  line-height: 20px;
  /* or 154% */

  text-align: right;
  letter-spacing: 0.06em;
  margin-bottom: 16px;
  color: #444343;
}
.gdp tbody tr:first-child {
  // text-align: left;text-indent: 1em;
  // color: #4570b6;
  // width: 100vw;
  /*结构上的第一个子元素，也就是将第一列单元格全都设置左对齐，添加缩进*/
}
#de {
  height: 30px;
  background-color: #82dbed;
  font-weight: 700;
  color: #373c38;
  text-align: center;
  /*设置“细节”单元格*/
}
td {
  height: 3vw;
  text-align: center;
  background-color: #f3fdff;
  /*设置表体单元格居中对齐*/
}
.gdp td,
th {
  width: 280px;
  border-top: solid 1px #dfdfdf;
  border-left: solid 1px #dfdfdf;
}

.gdp th {
  height: 40px;
  background: #5082c0;
  color: #fff;
  border-top: none;
}
.gdp tr:first-child,
.gdp th:first-child {
  border-left: none;
}
// .gdp tr:first-child::before{
//       content: '213';
// 			// position: absolute;
// 			width: 5px;
// 			height: 280px;
// 			top: 0; bottom: 0;margin: auto;
// 			border-width: 0 2px 2px 0;
// 			border-style: solid;
//       text-align: center;
//       justify-content: center;
// 			color: red;
// }
.gdp th {
  border-radius: 10px 10px 0 0;
  /*左表头的圆角*/
}
</style>
<style lang="scss">
.el-collapse-item__header.is-active {
  background-color: #4570b6 !important;
  color: #fff !important;
}
i {
  justify-content: space-between;
}
.el-collapse-item__arrow {
  display: none;
}
.el-collapse-item__header {
  font-weight: 400;
  font-size: 19px;
  height: 82px;
  background-color: #f3fdff;
  padding: 0 2vw;
  justify-content: space-between;
}
.el-collapse-item__content {
  font-weight: 400;
  font-size: 19px;
  padding: 2vw;
  background-color: #dfdfdf;
}
@media screen and (min-width: 768px) {
  .taoc_box_2 .box{
    
      margin-top: 35px !important;
    
  }
  .box:nth-child(1) img{
      height: 85px;
  }
  .box:nth-child(2) img{
    height: 85px;
  }
  .box:nth-child(3) img{
      height: 85px;
  }
  .box:nth-child(4) img{

    height: 85px;
  }
  .box:nth-child(5) img{

    height: 85px;
  }
  .box:nth-child(6) img{

    height: 85px;
  }

  .table-box_four{
    margin-top: 60px;
    margin-bottom: 100px;
    .table-head-blue{
      background-color: #5082C0;
      border-right: 0.5px solid #B3B1B2 !important;
      border-top: none !important;
      border-left: none !important;
      border-radius: 10px 10px 0px 0px;
      height: 68px !important;
      span{
        font-family: 'Noto Sans HK';
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 25px;
        /* or 139% */

        text-align: center;
        letter-spacing: 0.05em;

        color: #FFFFFF;
      }
    }
    .table-head-blue-2{
      background-color: #60A1CF;;
      border-right: 0.5px solid #B3B1B2 !important;
      border-top: none !important;
      border-left: none !important;
      border-radius: 10px 10px 0px 0px;
      height: 68px !important;
      span{
        font-family: 'Noto Sans HK';
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 25px;
        /* or 139% */

        text-align: center;
        letter-spacing: 0.05em;

        color: #FFFFFF;
      }
    }
    .boder-none{
          border: none !important;
          background-color:#fff !important;
          width: 103px !important;
    }
    .danyan{
      width: 73px !important;
      background-color: #5082C0;
      border-radius: 10px 0px 0px 10px;
      border: none !important;
      .text{
        font-family: 'Noto Sans HK';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 15px;
        /* or 75% */

        text-align: center;
        letter-spacing: 0.05em;

        color: #FFFFFF;
      }
    }
    .jiage{
      span{
        font-family: 'Noto Sans HK';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 15px;
        /* or 75% */

        text-align: center;
        letter-spacing: 0.05em;

        color: #444343;
      }
    }
    .free{
      .et2{
      background-color: #78CBE4;
      // border: 0.5px solid #B3B1B2;
      border-radius: 0px 0px 10px 10px;
      span{
        font-family: 'Noto Sans HK';
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 15px;
        /* identical to box height, or 83% */

        text-align: center;
        letter-spacing: 0.05em;

        color: #FFFFFF;
      }
      }
     
    }
  }




  .tab {
    margin: 50px auto;
    margin-top: 100px;
  }
  .taoc_box_2{
    .box{
      margin-top: 42px;
    }
    width: 553px !important;
    .icon-box {
      display: grid;
      grid-template-columns: repeat(2, 1fr) !important;
      justify-items: center;
    }
    .box span{
          line-height: 20px !important;
    }
    .shoufei{
      font-family: 'Noto Sans HK';
font-style: normal;
font-weight: 350;
font-size: 13px;
line-height: 20px;
/* identical to box height, or 154% */

letter-spacing: 0.06em;

color: #444343;
    }
  }
  .taoc_box {
    margin: 0 auto;
    width: 789px;
    height: 431px;
    background: #f5fdff;
    border: 0.5px solid #b3b1b2;
    border-radius: 10px;
    .icon-box {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      justify-items: center;
    }
    .box {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 49px;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 10px;
        /* or 50% */
        margin-top: 25px;
        text-align: center;
        letter-spacing: 0.05em;

        color: #444343;
      }
    }
    .titel {
      height: 39px;
      background: #5082c0;
      border: 0.5px solid #b3b1b2;
      border-radius: 10px 10px 0px 0px;
      display: flex;
      justify-content: center;
      align-items: center;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 15px;
        /* or 83% */

        text-align: center;
        letter-spacing: 0.05em;

        color: #ffffff;
      }
    }
  }
  #blue {
    height: 30px;
    background: #ffcccc;
    font-weight: 700;
    text-align: center;
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 500;
    font-size: 15px;
    line-height: 15px;
    /* or 100% */

    text-align: center;
    letter-spacing: 0.05em;

    color: #fb5e5e;
  }

  .free {
    height: 39px;
    background-color: #78cbe4 !important;

    border-radius: 0px 0px 10px 10px;
    font-weight: 500;
    color: #fff;
    text-align: center;
  }
  .table-1-box table tr td span {
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 400;
    font-size: 20px;
    line-height: 15px;
    /* or 75% */

    text-align: center;
    letter-spacing: 0.05em;

    color: #444343;
  }
  .gdp th p {
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 20px;
    /* or 83% */
    background-image: -webkit-linear-gradient(
      bottom,
      #fdfdfd,
      #ffffff
    ) !important;
    text-align: center;
    letter-spacing: 0.05em;

    color: #ffffff;
  }
  .taoc_boxs{
    span {
      letter-spacing: 0.02rem;

    }
  }
  .table-1-box {
    margin: 0 auto;
    margin-top: 60px;
    margin-bottom: 40px;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 350;
      font-size: 13px;
      line-height: 20px;
      /* or 154% */

      letter-spacing: 0.02rem;

      color: #444343;
    }
  }
  .tables {
    margin-top: 47px;
  }
  .tab-control .active {
    background-color: #ffffff;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 700;
      font-size: 18px;
      line-height: 15px;
      /* identical to box height, or 83% */

      text-align: center;
      letter-spacing: 0.1em;

      background: linear-gradient(90.69deg, #5082c0 8.74%, #78cbe4 95.29%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
    }
  }
  .tab-control {
    display: flex;
    justify-content: center;
    padding: 40px 0;
    cursor: pointer;
    .tab-control-item {
      padding: 0 30px;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 15px;
        /* identical to box height, or 83% */

        text-align: center;
        letter-spacing: 0.1em;

        color: #444343;
      }
    }
    .tab-control-item::after {
      content: "";
      margin-left: 34px;
      padding-left: 0;
      border-left: 1px solid #000;
      height: 17px;
      display: inline-block;
      vertical-align: middle;
    }
  }

  .contents {
    display: flex;
  }

  span {
    font-size: 14px;
  }
  .section_text {
    margin: 1vw 0;
  }
  .tab-control .tab-control-item:nth-child(4)::after {
    height: 0;
  }
}
@media screen and (max-width: 768px) {
  td{
    padding: 10px;
  }
  .taoc_box_2{
    .box span{
          line-height: 21px !important;
    }
  }
  .tab {
    margin: 50px auto;
  }
  .taoc_box {
    background: #f5fdff;
    border: 0.5px solid #b3b1b2;
    border-radius: 10px;
    padding-bottom: 49px;
    .box {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 49px;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 10px;
        /* or 50% */
        margin-top: 25px;
        text-align: center;
        letter-spacing: 0.05em;

        color: #444343;
      }
    }
    .titel {
      height: 39px;
      background: #5082c0;
      border: 0.5px solid #b3b1b2;
      border-radius: 10px 10px 0px 0px;
      display: flex;
      justify-content: center;
      align-items: center;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 15px;
        /* or 83% */

        text-align: center;
        letter-spacing: 0.05em;

        color: #ffffff;
      }
    }
  }
  #blue {
    height: 30px;
    background: #ffcccc;
    font-weight: 700;
    text-align: center;
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 500;
    font-size: 15px;
    line-height: 15px;
    /* or 100% */

    text-align: center;
    letter-spacing: 0.05em;

    color: #fb5e5e;
  }

  .free {
    height: 39px;
    background-color: #78cbe4 !important;

    border-radius: 0px 0px 10px 10px;
    font-weight: 700;
    color: #373c38;
    text-align: center;
  }
  .table-1-box table tr td span {
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 400;
    font-size: 20px;
    line-height: 15px;
    /* or 75% */

    text-align: center;
    letter-spacing: 0.05em;

    color: #444343;
  }
  .gdp th p {
    font-family: "Noto Sans HK";
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 20px;
    /* or 83% */
    background-image: -webkit-linear-gradient(
      bottom,
      #fdfdfd,
      #ffffff
    ) !important;
    text-align: center;
    letter-spacing: 0.05em;

    color: #ffffff;
  }
  .table-1-box {
    margin: 0 auto;
    margin-top: 20px;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 350;
      font-size: 13px;
      line-height: 20px;
      /* or 154% */

      letter-spacing: 0.06em;

      color: #444343;
    }
  }
  .tables {
    margin-top: 47px;
  }
  .tab-control .active {
    background-color: #ffffff;
    span {
      font-family: "Noto Sans HK";
      font-style: normal;
      font-weight: 700;
      font-size: 18px;
      line-height: 15px;
      /* identical to box height, or 83% */

      text-align: center;
      letter-spacing: 0.1em;

      background: linear-gradient(90.69deg, #5082c0 8.74%, #78cbe4 95.29%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-fill-color: transparent;
    }
  }
  .tab-control {
    display: flex;
    justify-content: center;
    padding-bottom: 40px;
    cursor: pointer;
    flex-direction: column;

    .tab-control-item {
      padding: 0 30px;
      text-align: center;
      span {
        font-family: "Noto Sans HK";
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 15px;
        /* identical to box height, or 83% */
        padding: 10px 0;
        text-align: center;
        letter-spacing: 0.1em;

        color: #444343;
      }
      hr {
        width: 172px;
        border-color: #000;
        margin-top: 10px;
        margin-bottom: 10px;
      }
    }
    .tab-control-item:nth-child(4) hr {
      display: none;
    }
    .tab-control-item {
      position: relative;
      margin: auto;
    }
  }

  .contents {
    display: flex;
  }

  span {
    font-size: 14px;
  }
  .section_text {
    margin: 1vw 0;
  }
  .tab-control .tab-control-item:nth-child(4)::after {
    height: 0;
  }
}
</style>
