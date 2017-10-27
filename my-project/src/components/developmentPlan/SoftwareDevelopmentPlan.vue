<template>
  <div id="software-development-plan" class="col-md-10 col-md-offset-2">
    <div class="glass-panel">
      <div class="main-items" >
        <div class="panel-list">
          <h6>前置条件</h6>
          <button class="button btn btn-info">上传</button>
        </div>
        <div class="panel-list">
          <h6>软件合格审定计划</h6>
          <button class="button btn btn-info">新建</button>
          <table class="table table-hover my-table">
            <thead>
              <tr>
                <th>#</th>
                <th>标识（编号）</th>
                <th>名称</th>
                <th>版本</th>
                <th>优先级</th>
                <th>重要程度</th>
                <th>状态</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>1</td>
                <td>Column content</td>
                <td>Column content</td>
                <td>Column content</td>
                <td>Column content</td>
                <td>Column content</td>
                <td>Column content</td>
              </tr>
            </tbody>
          </table> 
        </div>
        <div class="panel-list">
          <h6>软件开发计划</h6>
        </div>
        <div class="panel-list">
          <h6>软件验证计划</h6>
        </div>
        <div class="panel-list">
          <h6>软件配置管理计划</h6>
        </div>
        <div class="panel-list">
          <h6>软件质量保证计划</h6>
        </div>
        <div class="panel-list">
          <h6>软件需求标准</h6>
        </div>
        <div class="panel-list">
          <h6>软件设计标准</h6>
        </div>
        <div class="panel-list">
            <h6>软件编码标准</h6>
        </div>
      </div>
      <new-item class="panel-list new-item"></new-item>
    </div>
  </div>
</template>

<script>
import NewItem from './NewItem'
export default {
  name: 'SoftwareDevelopmentPlan',
  data(){
    return{
      show:false,
    }
  },
  components: {
    NewItem
  },
}
</script>

<style scoped>
#software-development-plan{
    float: left;
}
h6{
  color:#0073a8;
  font-weight: bold;
}
.panel-list h6{
  float: left;
}
.glass-panel{
  background-image: url('../../assets/img/box-bk2.png');
  margin:10px 20px;
  /* right: 50px; */
  padding:30px;
  border-radius:5px;
  position:absolute;
  width: 97%;
}
.panel-list{
    margin-bottom: 15px;
    float: left;
    padding: 0 30px ;
    background-color: #fff;
    min-height: 100px;
    border-radius: 7px;
    width: 100%;
}
.btn-info{
  font-size: 10px;
  float: right;
  margin:5px;
}
.my-table{
  background-color: #fff;
  color:#000;
  /* margin-top:10px; */
}
.my-table thead{
  padding: 5px 0 5px 5px;
  background-color: #E5E5E5;
  font-size: 14px;
  color: #3A3E55;
}
.table>tbody>tr>td{
  border-top:none;
  border-bottom:1px solid #ddd;

}
.my-table tbody tr:hover{
  background-color: #428bca;
}
.my-table thead th{
  border-left: solid 2px #fff;
  border-bottom: none;
}
.new-item{
  width: 90%;
}
</style>
