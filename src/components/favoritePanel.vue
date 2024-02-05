<template>
	<div>
		<favorite-card v-for="card in cardsListData" :key="card.id" :card-data="card"></favorite-card>
	</div>
</template>

<script>
import FavoriteCard from './favoriteCard.vue';

export default {
	name: 'FavoritePanel',
	components: { FavoriteCard },

	props: {
		cardsListData: {
			type: Array,
			default: () => []
		},
	},
}
</script>

<style lang="scss" scoped></style>