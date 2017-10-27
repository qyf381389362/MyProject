<template>
  <div id="new-item">
    <div class="panel-list">
      <h6>新建工作项</h6>
      <form class="form-horizontal new-item-form">
        <div class="form-group">
          <label for="inputEmail3">Email</label>
          <div>
            <input type="email" class="form-control" id="inputEmail3" placeholder="Email">
          </div>
        </div>
        <div class="form-inline form-group">
          <label for="InputName">类型：</label>
          <input type="text" class="form-control" id="InputName">
        </div>
        <button class="btn btn-info">新建并保存</button>
        <button class="btn">取消</button>
      </form>
      
    </div>
  </div>
</template>

<script>
export default {
  name: 'NewItem',
  components: {
    
  }
}
</script>

<style scoped>
h6{
  color:#0073a8;
  font-weight: bold;
}
.new-item-form{
  margin-top: 20px;
}
form label{
  color: #000;
}
.btn{
  border-radius: 50px;
  width:100px;
}
</style>
