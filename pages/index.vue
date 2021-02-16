<template>
  <div class="box">
    <el-container>
      <div class="boxs">
      <el-header style="height: 96px; width: 1248px"><Header></Header></el-header>
      <Banner style="height: 538px; width: 1248px"></Banner>
      <Introduce style="height: 3000px;; width: 1248px; background: pink"></Introduce>
      <el-footer style="height: 322px; width: 1248px"><Footer></Footer></el-footer>
      </div>
      <!-- <el-main>
          <Main>
            <Nuxt />
          </Main>
        </el-main> -->
    </el-container>
  </div>
</template>

<script>
import Header from "~/components/Header";
import Main from "~/components/Main";
import Footer from "~/components/Footer";
import "../assets/css/initialization.css";
import "../assets/css/normalize.css";
export default {
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style>
.boxs {
  margin: 0 auto;
  box-shadow: 5px 0px 5px -5px #ccc, -5px 0px 5px -5px #ccc;
}
.el-header {
  line-height: 96px;
}
.el-footer {
  line-height: 322px;
}

.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
  text-align: center;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}

body > .el-container {
  margin-bottom: 40px;
}
</style>