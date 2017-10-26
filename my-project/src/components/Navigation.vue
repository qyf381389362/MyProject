<template>
  <div id="navigation">
      <nav class="navbar navbar-inverse navbar-default navbar-fixed-top">
        <div class="container-fluid">
          <div class="navbar-header">
            <a class="navbar-brand" href="#">首&nbsp;&nbsp;&nbsp;&nbsp;页</a>
          </div>

          <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-2">
            <ul class="nav navbar-nav navlist">
              <li class="active list-item"><a href="#">活动配置<span class="sr-only">(current)</span></a></li>
              <li class="list-item"><a href="#">文档配置</a></li>
              <li class="list-item"><a href="#">角色配置</a></li>      
            </ul>
            <form class="navbar-form navbar-right" role="search">
              <div class="form-group">
                <input type="text" class="form-control" placeholder="搜索...">
              </div>
              <button type="submit" class="btn btn-default">搜索</button>
            </form>
          </div>
        </div>
      </nav>
  </div>
</template>

<script>
export default {
  name: 'navigation',
}
</script>

<style scoped>
#navigation{
  background: #222222;
  height: 52px;
}
.navbar-brand{
  padding-left: 60px;
  font-size: 18px;
}
.navlist{
  margin:0 50px;
  padding: 0 50px;
  font-size: 16px;
}
.list-item{
  margin:0 10px;
}
</style>
