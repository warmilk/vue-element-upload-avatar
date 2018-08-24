<template>
	<section>
		<button @click="dialogVisible = true">点我上传头像</button>
		<uploadAvatar :dialogVisible="dialogVisible" @on-close="closeDialog"></uploadAvatar>
	</section>
</template>

<script>
	import uploadAvatar from "@/components/uploadAvatar.vue"
	export default {
		data() {
			return {
				dialogVisible: false,
			}
		},
		components: {
			uploadAvatar
		},
		methods: {
			closeDialog() {
				this.dialogVisible = false
			}
		}
	};
</script>