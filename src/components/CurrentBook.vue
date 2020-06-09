<template>
	<div class="current-book panel">

		<img class="current-book-image" src="./../assets/images/covers/no-book.jpg" alt="Nic nečtu">

		<div class="current-book-detail">

			<p class="current-book-heading">Aktuálně čtu</p>
			<h2 class="current-book-title">Book Title</h2>
			<p class="current-book-meta">Author's Name, 1999</p>
			<p class="current-book-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente dicta ullam placeat facere omnis beatae mollitia? Minima culpa ut iure aliquid modi veniam, soluta temporibus qui at enim earum totam officia, ducimus, consequatur sit. Totam possimus earum harum iste aliquam.</p>

			<div class="current-book-actions">
				<button>Označit knihu jako přečtenou</button>
			</div>

		</div>
	</div>
</template>

<script>
export default {

}
</script>



<style>
.current-book {
	display: grid;
	grid-template-columns: minmax(120px, 180px) 2fr;
	gap: 30px;
}

.current-book-image {
	width: 100%;
	height: auto;
}

.current-book-heading {
	color: #888;
	font-weight: bold;
}

.current-book-title {
	margin-bottom: 10px;
}

.current-book-meta {
	margin-top: 10px;
	font-style: italic;
}

.current-book-description {
	margin-top: 24px;
	font-size: 85%;
	line-height: 1.5;
}
</style>