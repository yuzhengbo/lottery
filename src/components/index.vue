<template>
  <el-container>
    <el-header>
      <el-row type="flex" justify="center">
        <el-col :span="16" class="headerMain">
          <div class="logo">
            <img src="../assets/logo.png" alt="logo" height="40" width="40">
          </div>
          <div class="nickName">
            {{nickName}}
          </div>
          <div class="action">
            <span>教程</span>
            <el-switch
              v-model="value2">
            </el-switch>
          </div>
        </el-col>
      </el-row>
    </el-header>
    <el-main>
      main
    </el-main>
  </el-container>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      nickName: '阿比盖尔',
      money: '0.33',
      value2: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .el-header {
    background-color: #351743;
    color: #333;
    text-align: center;
    /*line-height: 60px;*/
    .headerMain {
      color: #fff;
      div {
        display: table-cell;
        vertical-align: middle;
        height: 60px;
        img {
          border-radius: 20px;
        }
      }
      .action {
        .el-switch,span {
          display: inline-block;
          color: #fff;
          vertical-align: middle;
          line-height: 60px;
          margin-right: 10px;
        }
      }
    }
  }
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }
</style>
