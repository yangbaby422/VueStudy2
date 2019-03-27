<template>
	<div class="container">
		<div class="side-bar">
			<router-link to="/task_id">任务编号</router-link>
			<router-link to="/task_type">类型</router-link>
			<router-link to="/task_name">任务名称</router-link>
			<router-link to="/export_time">导出时间</router-link>
			<router-link to="/task_status">状态</router-link>
			<router-link to="/file_size">文件大小</router-link>
			<router-link to="/operating">操作</router-link>
		</div>
		<div class="content"><router-view /></div>
	</div>
</template>

<script>
export default {
	name: 'Task',
	data() {
		return {
			
		};
	}		
};
</script>

<style scoped>
	.container {
		display: flex;
		width: 90%;
		margin: 0 auto;
		flex-direction: column;
	}
	.side-bar{
		flex: 1 1 20%;
		display: flex;
		background-color: #fff;
		margin-top: 20px;
	}
	a{
		margin-bottom: 30px;
	}
	.content{
		flex: 1 1 80%;
		text-align: left;
		background-color: #fff;
		margin-left: 20px;
		padding-bottom: 20px;
	}
</style>
