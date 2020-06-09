<template>
	<div class="book">
		<div class="book__image">
			<img src="./../assets/images/covers/no-book.jpg" alt="Obálka">
		</div>
		<div class="book__info">
			<h3 class="book__title">Book Title</h3>
			<p class="book__meta">Author's Name, 1999</p>
		</div>
		<div class="book__badges">
			<div class="book__badge book__badge--read">Přečteno</div>
			<div class="book__badge book__badge--current">Právě čtu</div>
		</div>
	</div>
</template>

<script>
export default {

}
</script>

<style>

.book {
  position: relative;
}

.book__image {
  padding: 0 20px;
}

.book__image img {
  width: 100%;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.15);
}

.book__info {
  text-align: center;
}

.book__title {
  font-size: 16px;
	line-height: 1.4;
	margin-bottom: 10px;
}

.book__meta {
  margin: 0;
  font-size: 14px;
  font-style: italic;
  color: #888;
}

.book__badges {
	position: absolute;
  top: 10px;
  left: 0px;
}

.book__badge {
  display: block;
  padding: 5px;
	margin-bottom: 5px;
  font-size: 13px;
  font-weight: bold;
  line-height: 1;
}

.book__badge--read {
  background-color: #bbb;
  color: #666;
}

.book__badge--current {
  background-color: tomato;
  color: white;
}


</style>