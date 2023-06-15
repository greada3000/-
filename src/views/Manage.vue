<template>
	<body id="poster">
		<el-container>
			<el-aside width="200px">
				<common-aside></common-aside>
			</el-aside>
			<el-container>
				<el-header style="background-color: antiquewhite;">
				
				<span><router-link target="_blank" :to="'/myhome/'+$store.getters.getUser.name ">{{ $store.getters.getUser.username }}</router-link></span>
				
				
				</el-header>
				<el-main>
					<router-view></router-view>
				</el-main>
			</el-container>
		</el-container>

	</body>
</template>

<script>
	import CommonAside from "../components/CommonAside.vue";
    export default {
        name: "Manage",
		components:{
			CommonAside
		}
    }
</script>

<style>



</style>