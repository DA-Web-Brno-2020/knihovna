<template>
  <div id="app">

    <h1>Knihovna</h1>

    <div class="library-top">
      <currentBook />
      <libraryInfo />
    </div>

    <libraryContent />

  </div>
</template>

<script>
import bookData from './assets/data/data.js';

import CurrentBook from './components/CurrentBook';
import LibraryInfo from './components/LibraryInfo';
import LibraryContent from './components/LibraryContent';

export default {
  name: 'App',

  components: {
    currentBook: CurrentBook,
    libraryInfo: LibraryInfo,
    libraryContent: LibraryContent
  },

  data() {
    return {
      books: bookData,
      aktualneCtu: 0
    }
  }

}
</script>

<style>
/* Google font */
@import url('https://fonts.googleapis.com/css2?family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&display=swap');

/* moderni box model */
html { box-sizing: border-box; }
*, ::after, ::before { box-sizing: inherit; }

/* základní styly */
body {
	font-family: 'Libre Baskerville', serif;
  margin: 0;
  padding: 1em;
	background: #f0ede6 url('./assets/images/background.png');
	background-blend-mode: multiply;
}

h1 {
  font-size: 48px;
  text-align: center;
}


.library-top {
	display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 30px;
  margin-bottom: 30px;
}

.panel {
	padding: 20px;
	background-color: rgba(255, 255, 255, 0.5);
}

button {
  flex: 1;
  margin-right: 10px;
  padding: 0.5em 1em;
  font-family: 'Libre Baskerville', serif;
  font-size: 15px;
  text-align: center;
  border: 1px solid black;
  border-radius: 4px;
  cursor: pointer;
  background-color: lightgray;
  color: black;
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.2);
  outline: 0;
}

button:hover {
  background-color: black;
  color: white;
}

button:active {
  transform: translateY(2px);
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.3);
}



.table {
	width: 100%;
	border-collapse: collapse;
}

.table td {
	border: 1px solid black;
	padding: 10px;
}

.table td:nth-child(2) {
	font-weight: bold;
}

</style>
