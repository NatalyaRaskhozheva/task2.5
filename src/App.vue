<template>
	<favorite-panel :cards-list-data="items"></favorite-panel>
</template>

<script>
import FavoritePanel from "./components/favoritePanel.vue";
import { items } from "./constants/data_items"
export default {
	name: 'App',
	components: {
		FavoritePanel
	},
	data() {
		return {
			items
		}
	}
}
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
