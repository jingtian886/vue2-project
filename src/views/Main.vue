<template>
  <div>
    <el-container>
      <el-aside width="auto">
        <CommonAside></CommonAside>
      </el-aside>
      <el-container>
        <el-header>
          <CommonHeader></CommonHeader>
        </el-header>
        <CommonTag></CommonTag>
        <el-main>
          <router-view></router-view>

        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import CommonAside from '../components/CommonAside.vue'
import CommonHeader from '../components/CommonHeader.vue'
import CommonTag from '../components/CommonTag.vue'
export default {
  data() {
    return {

    }
  },
  components: {
    CommonAside,
    CommonHeader,
    CommonTag
  }
}
</script>

<style>
.el-container {
  height: 100vh;
}
.el-header {
  background-color: #333;
}
.el-main {
  height: 100%;
}
</style>