<template lang='pug'>
.w-full.h-full.bg-yellow-100.font-sans(
	class="px-2 py-2 md:px-24 md:py-24"
)
	.w-full.border.rounded.border-gray-900.px-8.py-8
		h1.text-6xl IC
		.max-w-lg
			p.mt-8 You're viewing a super early alpha, we'll fix the UI in a bit.
			p.mt-6 The Internet Committe keeps the network stable and makes applications for the people of IIITB.
		
		
		a(
			href="mailto:ic@iiitb.org"
		)
			button.inline Contact

		routerLink(
			to="/members"
		)
			button.inline.ml-4 Members


		
	.w-full
		a(
			href="https://iiitb.me"
		) 
			button.inline iiitb.ME
		
		a(
			href="https://ic.iiitb.me"
		)
			button.inline.ml-6 IC | Beta

		a(
			href="https://menu.iiitb.me"
		) 
			button.inline.ml-6 Menu | Beta

		
</template>

<style scoped>
button {
	@apply border border-gray-900 rounded px-4 py-2 mt-8;
	outline: none;
}

button:active {
	@apply bg-gray-900 text-gray-100;
}
</style>

<script>
import Avatar from '@/components/Avatar.vue';

export default {
	name: 'home',
	components: {
		Avatar
	}
}
</script>
