<template>
	<div class="container">
		<h1>新建分类</h1>
		<el-form label-width="120px" :model="model" @submit.native.prevent="save">
			<el-form-item label="名称">
				<el-input v-model="model.name"></el-input>
			</el-form-item>
			<el-form-item label="名称">
				<el-button type="primary" native-type="submit">保存</el-button>
			</el-form-item>
		</el-form>
	</div>
</template>
<script>
export default {
	data() {
		return {
			model: {}
		};
	},
	methods: {
		save() {
			console.log(1);
			this.$http.post().then(() => {});
		}
	}
};
</script>

<style lang="scss" scoped>
</style>
