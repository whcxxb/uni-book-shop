<template>
	<view class="content">
		首页
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
	async	onLoad() {
		 // const data = await this.$u.get('/api/index')
		 // console.log(data)
		 // console.log(2222)
		 
		 // const data = await this.$u.get('/api/orders/1/confirm',{name:'liming'})
		 // const res = await this.$u.api.index()
		 // console.log(res)
		 const data = {
			 email:'test@a.com',
			 password:123123
		 }
		 const res = await this.$u.api.authLogin()
		 console.log(res)
		},
		methods: {

		}
	}
</script>

<style lang="scss" scoped>
	
</style>
