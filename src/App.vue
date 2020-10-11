<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat+Alternates&display=swap');
*{
	box-sizing: border-box;
	font-family: Montserrat, Helvetica, Arial, sans-serif;
}
#app {
	border-style: hidden;
	border-radius: 0;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	background-color: #FCF6F5FF;
	width: inherit;
	min-width: 40rem;
}
#home {
	border-style: hidden;
	border-radius: 0;
}

button {
	border-radius: 1rem;
	background-color: gold;
	box-shadow: none;
	border: none;
	cursor: pointer;
	font-size: 2rem;
	color: white;
	margin: 1rem;
}

button:hover {
	background-color: white;
	color: gold;
}

h1 {
	font-family: Pacifico, cursive;
	font-size: 5rem;
	color: #990011FF;
}
h2 {
	color: #000000;
	font-style: italic;
	background-color: #FFFFFF;
	display: block;
	margin-left: auto;
	margin-right: auto;
	border-radius: 1rem;
	width: 33%;
}

div {
	border-width: 1px;
	border-radius: 1rem;
	border-color: #880000DD;
	border-style: solid;
	width: 100%;
	overflow-x: auto;
	padding-bottom: 5rem;
}

.song-choice-container {
	padding: 1rem;
}


</style>