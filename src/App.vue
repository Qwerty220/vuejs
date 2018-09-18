<template>
  <div id="app">
	  <el-table
		:data="tableData"
		border
		style="width: 100%">
		<el-table-column
		  prop="date"
		  label="Date"
		  width="180">
		</el-table-column>
		<el-table-column
		  prop="name"
		  label="Name"
		  width="180">
		</el-table-column>
		<el-table-column
		  prop="address"
		  label="Address">
		</el-table-column>
	  </el-table>
  </div>
</template>

<script lang="ts">
    import { Vue, Component, Prop } from "vue-property-decorator";

    @Component
    export default class App extends Vue {

	tableData = [{
          date: '2016-05-03',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-02',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-04',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-01',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }];
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
