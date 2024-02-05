<template>
	<div class="container">
		<div class="img_container">
			<img :src="cardData.imgSrc" alt="">
		</div>
		<div class="product_info">
			<h2>{{ cardData.titleProduct }}</h2>
			<p>{{ cardData.discount }}</p>
		</div>
		<div class="product_buy">
			<h1>{{ cardData.price }}</h1>
			<button>Купити</button>
		</div>
	</div>
</template>

<script>
export default {
	name: 'FavoriteCard',
	props: {
		cardData: {
			type: Object,
			default: () => ({})
		},
	},
}
</script>

<style lang="css" scoped>
.container {
	display: inline-block;
}

img {
	width: 50%
}
</style>