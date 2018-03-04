<template>
	<div>
		<h1>No setting</h1>
		<br />
		<carousel
			:autoplay="true"
			:loop="true"
			per-page="3"
			pagination-color="#4b4b4b"
		>
			<slide v-for="number in 9" :key="number">
				Slide #{{ number }}
			</slide>
		</carousel>
		<h1>Set to true</h1>
		<br />
		<carousel
			:autoplay="true"
			:loop="true"
			:scroll-per-page="true"
			per-page="3"
			pagination-color="#4b4b4b"
		>
			<slide v-for="number in 9" :key="number">
				Slide #{{ number }}
			</slide>
		</carousel>
		<h1>Set to false</h1>
		<br />
		<carousel
			:autoplay="true"
			:loop="true"
			:scroll-per-page="false"
			per-page="3"
			pagination-color="#4b4b4b"
		>
			<slide v-for="number in 9" :key="number">
				Slide #{{ number }}
			</slide>
		</carousel>
	</div>
</template>

<script>
export default {
	name: 'app',
	data() {
		return {
			message: 'Welcome to Your Vue.js App',
		};
	},
};
</script>

<style>
body {
	font-family: Arial;
}

.VueCarousel-slide {
	background: #42b983;
	color: #fff;
	font-size: 24px;
	text-align: center;
	padding: 2.5em 0;
	border-right: 1px solid rgba(255, 255, 255, 0.25);
	box-sizing: border-box;
}
</style>
