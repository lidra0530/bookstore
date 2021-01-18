<template>
  <div class="home" id="home" name="home">
    <!-- 轮播图 -->
    <div class="block">
      <el-carousel height="350px">
        <el-carousel-item v-for="item in carousel" :key="item.carousel_id">
          <img
            style="height: 350px"
            :src="item.imgPath"
            :alt="item.describes"
          />
        </el-carousel-item>
      </el-carousel>
    </div>
    <!-- 轮播图END -->
    <div class="main-box">
      <div class="main">
        <!-- 商品展示区 -->
        <div class="phone">
          <div class="box-hd">
            <div class="title">书本推荐</div>
          </div>
          <div class="box-bd">
            <div class="list">
              
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      carousel: [
        {
          carousel_id: 1,
          describes: "123456",
          imgPath: require("../assets/imgs/1.jpg"),
        },
        {
          carousel_id: 2,
          describes: "123456",
          imgPath: require("../assets/imgs/2.jpg"),
        },
        {
          carousel_id: 3,
          describes: "123456",
          imgPath: require("../assets/imgs/3.jpg"),
        },
        {
          carousel_id: 4,
          describes: "123456",
          imgPath: require("../assets/imgs/4.jpg"),
        },
        {
          carousel_id: 5,
          describes: "123456",
          imgPath: require("../assets/imgs/5.jpg"),
        },
      ],
      goodslist: [{}],
    };
  },
};
</script>

<style>
@import "../assets/css/index.css";
</style>