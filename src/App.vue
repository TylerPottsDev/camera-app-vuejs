<template>
	<div id="app">
		<img alt="Vue logo" src="./assets/logo.png">
		<video autoplay></video>
	</div>
</template>

<script>
export default {
	name: 'app',
	components: {},
	data: function () {
		return {
			stream: null
		}
	},
	methods: {
		init: async function () {
			// if ('mediaDevices' in navigator && 'getUserMedia' in navigator.mediaDevices) {
			// 	let constraints = {
			// 		video: {
			// 			width: { min: 1280 },
			// 			height: { min: 720 }
			// 		},
			// 	};

			// 	const stream = await navigator.mediaDevices.getUserMedia(constraints);

			// 	const video = document.querySelector('video');
			// }
		},
		getDevices: async function () {
			// const devices = await navigator.mediaDevices.enumerateDevices();
		}
	},
	beforeMount: function () {
		this.init();
	}
}
</script>

<style>
video {
	width: 100%;
	background: rgba(0, 0, 0, 0.2);
}
</style>
