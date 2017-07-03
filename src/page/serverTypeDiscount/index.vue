<template>
  <div class="serverTypeDiscount">
    <el-row>
      <el-col :span="2" class="import-font">关键字：</el-col>      
      <el-col :span="10">
          <el-input :span="10" v-model="input" size="large" placeholder="请输入支付宝绑定的手机号/订单号/运单号"></el-input>
      </el-col>
      <el-col :span="4" class="import-search">
        <el-button type="primary" size="large">搜 索</el-button>
      </el-col>   
    </el-row>
  </div>

</template>
<script>
  export default {
    name:'serverTypeDiscount',
    data() {
      return {
        input: ''
      }
    }
  };
</script>

<style>
.import-font{
  height:42px;
  line-height: 42px;
}
.order-input{
  width: 500px;
}
.import-search{
  margin-left: 20px;
}

</style>

