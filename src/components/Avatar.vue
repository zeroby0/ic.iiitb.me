<template lang='pug'>
figure.border.border-gray-900.rounded.px-4.py-4.w-32.mt-4.mr-4
	img(
		:src="'/img/avatars/' + photo + '.jpg'"
	).rounded-full.overflow-none.h-12.w-12.mx-auto.object-cover.object-center
	p.mt-4.text-center {{name}}


		
</template>

<style scoped>
img {
	-webkit-filter: grayscale(100%); /* Safari 6.0 - 9.0 */
	filter: grayscale(100%);
}
</style>

<script>

export default {
	name: 'home',
	props: [
		'name',
		'photo'
	],
	computed: {
		photoURL: function() {
			return '/img/assets/avatars/' + this.photo + '.jpg'
		}
	}
}
</script>
