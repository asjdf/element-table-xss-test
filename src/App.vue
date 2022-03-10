<template>
  <el-table :data="tableData" style="width: 100%">
    <el-table-column prop="date" label="Date" />
    <el-table-column prop="name" label="Name" />
    <el-table-column show-overflow-tooltip prop="address" label="Address" width="100"/>
  </el-table>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      tableData: [{
        date: '2016-05-03',
        name: 'Tom',
        address: '<img src=https://eson.ninja/img/reol.png onload=alert(1)>',
      }]
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
