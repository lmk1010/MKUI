<template>
    <div class="page-header">
        <div class="page-header-image" style="background-image:url(../../../static/images/login.jpg)"></div>
         <div class="container">
        <div class="col-md-12 content-center">
            <div class="card-plain">
                <form class="form" method="" action="">
                    <div class="header">
                        <div class="logo-container">
                            <img src="../../../static/images/logo.svg" alt="">
                        </div>
                        <h5>MKOS</h5>
                    </div>
                    <div class="content">                                                
                        <div class="input-group input-lg">
                            <input type="text" class="form-control" placeholder="账户">
                            <span class="input-group-addon">
                                <i class="zmdi zmdi-account-circle"></i>
                            </span>
                        </div>
                        <div class="input-group input-lg">
                            <input type="password" placeholder="口令" class="form-control" />
                            <span class="input-group-addon">
                                <i class="zmdi zmdi-lock"></i>
                            </span>
                        </div>
                    </div>
                    <div class="footer text-center">
                        <a href="index.html" class="btn btn-primary btn-round btn-lg btn-block ">LOG IN</a>
                    </div>
                </form>
            </div>
        </div>
    </div>
        <footer class="footer">
            <div class="container">
                <nav>
                    <ul>
                        <li><a href="#" target="_blank">Contact Us</a></li>
                        <li><a href="#" target="_blank">About Us</a></li>
                        <li><a href="javascript:void(0);">FAQ</a></li>
                    </ul>
                </nav>
                <div class="copyright">
                    &copy;
                    <span>Resloved by <a href="#" target="_self">MK</a></span>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>

export default {
  name: "login",
  methods: {
    onSubmit() {
      window.location.href="index.html"
      // this.$notify({
      //   title: "成功",
      //   message: "这是一条成功的提示消息",
      //   type: "success"
      // });
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
  width: 100%;
}
.el-footer {
  position: relative;
  bottom: 0;
  width: 100%;
  height: 100px;
}
</style>
