<template>
	<div class="challenge">
		<div class="mt-24">
			<img class="like" :class="moveIt" src="/img/like.png" />
		</div>

		<b-button @click="switchLoading" type="is-primary">{{btnText}}</b-button>
	</div>
</template>

<script>
export default {
	name: "Challenge",

	data: () => ({
		isLoading: true
	}),

	methods: {
		switchLoading() {
			this.isLoading = !this.isLoading;
		}
	},

	computed: {
		btnText(evt) {
			return this.isLoading ? "stop" : "start";
		},

		moveIt(evt) {
			return this.isLoading ? "rotate" : "";
		}
	}
};
</script>

<style scoped>
	.challenge {
		text-align: center;
	}

	.like {
		width: 6rem;
		margin-bottom: 4rem;
	}

	.rotate {
		animation: rotation 2s infinite linear;
	}

	@keyframes rotation {
		from {
			transform: rotate(0deg);
		}
		to {
			transform: rotate(359deg);
		}
	}
</style>
