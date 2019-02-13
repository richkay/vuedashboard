<template>
  <el-container>
    <el-aside width="200px">
        <div class="logo"><h1>KarmaHUB</h1></div>
    </el-aside>
    <el-container>
        <el-header>
          <comheader />
        </el-header>
        <el-main><nuxt/></el-main>
    </el-container>
  </el-container>
</template>

<script>
import comheader from '~/components/layout/header'

export default {
  name: 'default',
  components: {
    comheader
  },

}
</script>


<style>
html
{
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
*, *:before, *:after
{
  box-sizing: border-box;
  margin: 0;
}
</style>
