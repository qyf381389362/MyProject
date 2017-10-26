<template>
  <div id="stacked-navigation">
    <div class="container-fluid">
      <div class="row">
        <div class="col-md-2 sidebar">
          <ul class="nav nav-sidebar">
            <li class="active">
              <a href="#">项目策划阶段 <span class="sr-only">(current)</span></a>
              <ul class="nav nav-child">
                <li>软件研制任务书框架讨论</li>
                <li>编写软件研制任务书</li>
                <li>项目策划阶段技术评审</li>
                <li>功能基线建立并发布</li>
              </ul>
            </li>
            <li>
              <a href="#">软件计划阶段</a>
              <ul class="nav nav-child hide">
                <li>软件研制任务书框架讨论</li>
                <li>编写软件研制任务书</li>
                <li>项目策划阶段技术评审</li>
                <li>基线建立并发布</li>
              </ul>
            </li>
            <li>
              <a href="#">软件需求阶段</a>
            </li>
            <li><a href="#">软件设计阶段</a></li>
            <li><a href="#">软件编码阶段</a></li>
            <li><a href="#">集成与测试阶段</a></li>
            <li><a href="#">高层需求测试用例设计阶段</a></li>
            <li><a href="#">低层需求测试用例设计阶段</a></li>
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
    return{
    
    }
  },
  methods:{
    showTabs:function(){
       
    }
  },
  
}
</script>

<style scoped>
.sidebar{
  position: fixed;
  top:52px;
  bottom:0;
  left: 0;
  /* z-index: 1000; */
  display: block;
  padding:20px;
  overflow-x: hidden;
  overflow-y: auto;
  background-color: #f5f5f5;
  border-right: 1px solid #ddd;
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
}
.nav-child li{
  margin:10px;
}
</style>
