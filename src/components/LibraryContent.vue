<template>
	<div class="library-content panel">

		<div class="library-content-actions">
			<span class="actions-label">Zobrazit</span>
			<button>Všechny knihy</button>
			<button>Nepřečtené knihy</button>
			<button>Přečtené knihy</button>
		</div>

		<div class="library-content-list">

			<book />
			<book />
			<book />
			<book />
			<book />

		</div>
	</div>
</template>

<script>
import Book from './Book.vue';

export default {
	components: {
		book: Book
	}
}
</script>

<style>
.library-content-actions {
	margin-bottom: 40px;
}

.actions-label {
	color: #888;
	font-weight: bold;
	margin-right: 20px;
}

.library-content-list {
  display: grid;
  grid-gap: 30px;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
}
</style>