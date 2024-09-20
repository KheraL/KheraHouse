<template>

  <div class="topImag">
    <img class="openImag" src="./assets/bgImg.png">
    <div class="preparebox">
      <img class="identification" src="./assets/iden.png">
      <div class="openaccount-btn" @click="openAccount">
        <div class="openimmedia">立即开户</div>
        <div class="availbletime">网上开户时间为交易日09:00 - 11:29、13:00 - 16:55</div>
      </div>
    </div>
    <img class="needhelptext" src="./assets/needhelp.png">

    <div class="bottomarea helplistbox">
      <div class="helpbtn" @click="openCommonIsuuePage">
        <img class="helpbtnimg" src="./assets/commonIssue.png">
        <div class="helpbtntext">常见问题</div>
      </div>

      <div class="helpbtn" @click="openBankLinkGuidePage">
        <img class="helpbtnimg" src="./assets/guidlead.png">
        <div class="helpbtntext">银期签约指南</div>
      </div>

      <div class="helpbtn" @click="callHotLine">
        <img class="helpbtnimg" src="./assets/hotline.png">
        <div class="helpbtntext">客服热线</div>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  methods: {
    openAccount() {
      window.location.href = 'https://saas.kingsteching.com/h5/#/no_back/318fc35bc49c44b6/SIM_CONTEST_QH/detail/543';
    },
    callHotLine(){
      window.location.href = 'tel://' + 4008209128
    }

  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
}
.topImag {
  background: #f8f8f8;
}
.topImag .openImag {
  width: 100%;
  height: 400px;
  
}
img {
  display: block;
}

.topImag .preparebox{
  width:331px;
  height: 200px;
  background: #ffffff;
  border-radius: 15px;
  margin-left: 15px;
  position: relative;
  bottom: 120px;
  overflow: hidden;
}

.topImag .identification {
  width: 220px;
  height: 83px;
  margin-top: 10px;
  margin-left: 60px;
}

.topImag .openaccount-btn {
  background: rgb(243, 93, 18);
  width: 290px;
  height: 44px;
  margin-top: 18px;
  margin-left: 19px;
  border-radius: 27px;
  font-weight: 500;/*用于设置文本粗细*/
  font-size: 17px;
  color:#ffffff;
  display: flex;
  align-items: center;
  flex-direction: column;
  font-family: PingFangSC, PingFang SC;
}

.topImag .openimmedia {
  line-height: 22px;
  margin-top: 10px;
}

.topImag .availbletime {
  font-weight: 400;
  font-size: 11px;
  color: #777;
  line-height: 16px;
  text-align: center;
  margin-top: 17px;
  font-family: PingFangSC, PingFang SC;
}

.topImag .needhelptext {
  width: 273px;
  height: 20px;
  position: relative;
  bottom: 80px;
  margin-left: 47px;
}



.topImag .bottomarea {
  margin-left: 78px;
  margin-right: 79px;
}

.topImag .helplistbox {
  display: flex;
  justify-content: space-between;
  position: relative;
  bottom: 48px;
}

.topImag .helpbtn {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.topImag .helpbtnimg {
  width: 42px;
  height: 42px;
}

.topImag .helpbtntext {
  font-family: PingFangSC,PingFang SC;
  font-weight: 400;
  font-size: 12px;
  color: #777;
  line-height: 18px;
  margin-top: 8px;
}
</style>
