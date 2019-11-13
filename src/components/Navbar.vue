<template lang='pug'>
Nav.w-full.h-12.flex.justify-between.px-4.py-2.bg-yellow-400.text-gray-900.align-middle
	.left.inline.flex
		router-link(
			to="/"
		).my-auto IC

	.right.inline.flex
		router-link(
			to="/members"
		).my-auto Members
</template>

<style lang="postcss" scoped>
</style>

<script>
export default {
  name: 'Navbar',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
