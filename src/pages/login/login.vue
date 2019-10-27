<template>
 <el-container>
    <el-header height="100px">
      <div>
        <el-row :gutter="3">
          <el-col :sm="{span:6,offset:9}" :xs="{span:12,offset:6}">
            <el-image :src="logo"></el-image>
          </el-col>
        </el-row>
      </div>
    </el-header>
    <el-main>
      <el-form ref="login_form">
        <el-row :gutter="3">
          <el-col :sm="{span:8,offset:8}" :xs="{span:24}">
            <el-form-item>
              <el-input type="text" v-model="login_name" placeholder="请输入用户名"></el-input>
            </el-form-item>
          </el-col>
        </el-row>
        <el-row :gutter="3">
          <el-col :sm="{span:8,offset:8}" :xs="{span:24}">
            <el-form-item>
              <el-input type="password" placeholder="请输入密码" v-model="pass_word"></el-input>
            </el-form-item>
          </el-col>
        </el-row>
        <el-row :gutter="3">
          <el-col :sm="{span:8,offset:8}" :xs="{span:32}">
            <el-form-item>
              <el-button style="width:450px" size="medium" type="primary" @click="onSubmit" round>登陆</el-button>
            </el-form-item>
          </el-col>
        </el-row>
      </el-form>
    </el-main>
    <el-footer>
      <div>
        <el-row :gutter="3">
          <el-col :sm="{span:9,offset:8}" :xs="{span:24}">
            <p>All CopyRight By Lmk Resloved！Since By 2019-2030 @Nexus Industry</p>
          </el-col>
        </el-row>
      </div>
    </el-footer>
  </el-container>
</template>

<script>

import logo from './assets/Logo.png'

export default {
  name: "login",
  data: function() {
    return {
      login_name: "",
      pass_word: "",
      logo:logo
    };
  },
  methods: {
    onSubmit() {
      this.$notify({
        title: "成功",
        message: "这是一条成功的提示消息",
        type: "success"
      });
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.el-header {
  margin-top: 120px;
}
.el-main {
  position: relative;
  margin-top: 30px;
}
.el-button {
  position: relative;
  margin-top: 30px;
}
.el-footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 100px;
}
</style>
