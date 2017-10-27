<template>
  <div id="stacked-navigation">
    <div class="container-fluid">
      <div class="row">
        <div class="col-md-2 sidebar glass-panel">
          <ul class="nav nav-sidebar">
            <li>
              <a href="#">项目策划阶段 <span class="sr-only">(current)</span></a>
              <ul class="nav nav-child">
                <li><a href="#">软件研制任务书框架讨论</a></li>
                <li><a href="#">编写软件研制任务书</a></li>
                <li><a href="#">项目策划阶段技术评审</a></li>
                <li><a href="#">功能基线建立并发布</a></li>
              </ul>
            </li>
            <li>
              <a href="#">软件计划阶段</a>
              <ul class="nav nav-child">
                <li><a href="#">编写计划过程</a></li>
                <li><a href="#">核查计划过程</a></li>
                <li><a href="#">评审计划过程</a></li>
                <li><a href="#">计划过程配置管理</a></li>
                <li><a href="#">计划过程质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul>
            </li>
            <li>
              <a href="#">软件需求阶段</a>
              <ul class="nav nav-child">
                <li><a href="#">构建高层需求</a></li>
                <li><a href="#">核查高层需求</a></li>
                <li><a href="#">评审高层需求</a></li>
                <li><a href="#">高层需求配置管理</a></li>
                <li><a href="#">高层需求质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul>
            </li>
            <li>
              <a href="#">软件设计阶段</a>
              <ul class="nav nav-child">
                <li><a href="#">构建低层需求和架构设计</a></li>
                <li><a href="#">核查软件设计</a></li>
                <li><a href="#">评审软件设计</a></li>
                <li><a href="#">低层需求配置管理</a></li>
                <li><a href="#">低层需求质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul>
            </li>
            <li>
              <a href="#">软件编码阶段</a>
              <ul class="nav nav-child">
                <li><a href="#">软件编码</a></li>
                <li><a href="#">核查软件编码</a></li>
                <li><a href="#">评审软件编码</a></li>
                <li><a href="#">软件编码配置管理</a></li>
                <li><a href="#">软件编码质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul>
            </li>
            <li>
              <a href="#">集成过程</a>
              <ul class="nav nav-child">
                <li><a href="#">集成</a></li>
                <li><a href="#">核查集成</a></li>
                <li><a href="#">评审集成</a></li>
                <li><a href="#">集成配置管理</a></li>
                <li><a href="#">集成质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul>
            </li>
            <li>
              <a href="#">高层需求测试用例设计阶段</a>
              <ul class="nav nav-child">
                <li><a href="#">测试用例设计</a></li>
                <li><a href="#">核查测试用例设计</a></li>
                <li><a href="#">评审测试用例设计</a></li>
                <li><a href="#">测试用例设计配置管理</a></li>
                <li><a href="#">测试用例设计质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul>
            </li>
            <li>
              <a href="#">低层需求测试用例设计阶段</a>
              <ul class="nav nav-child">
                <li><a href="#">测试用例设计</a></li>
                <li><a href="#">核查测试用例设计</a></li>
                <li><a href="#">评审测试用例设计</a></li>
                <li><a href="#">测试用例设计配置管理</a></li>
                <li><a href="#">测试用例设计质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul> 
            </li>
            <li>
              <a href="#">集成测试</a>
              <ul class="nav nav-child">
                <li><a href="#">集成测试设计</a></li>
                <li><a href="#">核查集成测试设计</a></li>
                <li><a href="#">评审集成测试设计</a></li>
                <li><a href="#">集成测试配置管理</a></li>
                <li><a href="#">集成测试质量保证</a></li>
                <li><a href="#">基线建立并发布</a></li>
              </ul>
            </li>
            <li><a href="#">软件总结阶段</a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import $ from 'jquery'

export default {
  name: 'StackedNavigation',
  data(){
    return{}
  },
  methods:{
    showTabs:function(){
    }
  },
}
  $(function(){
    var $nav_li = $(".nav.nav-sidebar>li");
    $nav_li.click(function(){
      $(this).addClass("active")
              .siblings().removeClass("active");
      $(this).children('ul').show()
              .parent().siblings().children('ul').hide();

    });
  });
</script>

<style scoped>
.sidebar{
  position: absolute;
  top:52px;
  bottom:0;
  left: 0;
  /* z-index: 1000; */
  display: block;
  padding:20px;
  overflow-x: hidden;
  overflow-y: auto;
  /* background-color: #f5f5f5; */
  border-right: 1px solid #ddd;
  float: left;
}
.nav-sidebar {
  margin-right: -21px; /* 20px padding + 1px border */
  margin-bottom: 20px;
  margin-left: -20px;
}
.nav-sidebar > li > a {
  padding-right: 20px;
  padding-left: 20px;
}
.nav-sidebar > .active > a,
.nav-sidebar > .active > a:hover,
.nav-sidebar > .active > a:focus {
  color: #fff;
  background-color: #0073a8;
}
.nav-child{
  font-size: 15px;
  margin:5px 50px;
  color:#7f8c8d;
  display:none;
}
.nav-child li{
  margin:10px;
}
.nav-child li a{
  margin:2px 0;
  padding: 2px;
  /* color:#7f8c8d; */
  color:#000;
  font-size:12px;
}
.glass-panel{
  background-image: url('../assets/img/box-bk2.png');
  background-position: no-repeat;
  margin:10px 20px;
  padding:30px;
  border-radius:5px;
  position:absolute;
}
</style>
