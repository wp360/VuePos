<template>
  <div class="pos">
      <el-row>
          <el-col :span='7' class="pos-order" id="order-list">
              订单栏区域
          </el-col>
          <el-col>
              产品栏区域
          </el-col>
      </el-row>
  </div>
</template>
<script>
    export default{
        name: 'pos',
        mounted: function(){
            var orderHeight = document.body.clientHeight;
            //console.log(orderHeight);
            document.getElementById('order-list').style.height = orderHeight + 'px';
        }
    }
</script>
<style scoped>
    .pos-order{
        background-color: #F9FAFC;
        border: 1px solid #C0CCDA;
        height: 100%;
    }
</style>

