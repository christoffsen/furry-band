<template>
	<div id="home">
		<h1>Roadtrippers</h1>
		<div class="song-choice-container">
			<button v-for="song in songs" :key="song.name" @click="changeSong(song)">{{song.name}}</button>
		</div>
		<div v-if="currentSong !== null">
			<h2>{{currentSong.name}}</h2>
			<video controls width="800" height="600" :src="currentSong.link" type="video/mp4"></video>
		</div>
	</div>
</template>

<script>
// @ is an alias to /src

export default {
	name: 'Home',
	data() {
		return {
			currentSong: null,
			songs: [
				{"name" : "Locomotive Breath", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/Locomotive_Breath.mp4"}
				,{"name" : "Proud Mary", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/Proud_Mary.mp4"}
				,{"name" : "I Saw Her Standing There", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/I_Saw_Her_Standing_There.mp4"}
				,{"name" : "Last Kiss", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/Last_Kiss.mp4"}
				,{"name" : "Keep on Runnin'", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/Keep_on_Runnin.mp4"}
				,{"name" : "No Matter What", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/No_Matter_What.mp4"}
				,{"name" : "Dead Flowers", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/Dead_Flowers.mp4"}
				,{"name" : "I Hear You Knocking", "link" : "https://band-videos.s3.ca-central-1.amazonaws.com/I_Hear_You_Knocking.mp4"}
			]
		}
	},
	methods: {
		changeSong(song) {
			this.currentSong = song;

		}
	},
	components: {
	}
}
</script>