<template>
  <div class="common-layout">
    <el-container>
      <el-aside width="200px" class="left-title">
        <ul>
          <li>羽毛球</li>
        </ul>
      </el-aside>
      <el-container>
        <el-header>Header</el-header>
        <el-main>Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {}
}
</script>

<style>
body {
  margin: 0;
}

.left-title li{
  list-style-type: none;
}
</style>
