<script>
	export let name;
</script>

<main>

	<div class="container">
		<div class="circleHolder">
			<div class="circle-animation"></div>

		</div>

		<span class="random-fact"></span>
		

	</div>
	
</main>

<style>
	main {
		text-align: center;
		padding: 0;
		max-width: 240px;
		margin: 0;
	}

	/* .random-fact {
		width: 100px;
		height: 100px;
		background: white;
		
	} */


	.container {
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		height: 100vh;
		background: aquamarine;
	}
	.circle-animation {
		margin-top: -1rem;
		width: 400px;
		height: 400px;
		/* background-image: url('/ProfilePic.png'); */
		background-color:rgb(111,138,32);
		background-size: 400px;
		align-self: center;
		border-radius: 50%;
		border: none;
		animation: breathe 8s linear infinite;
	}

	@keyframes breathe {
		0% {
			box-shadow: 0 0 0 15px rgba(111,138,32, 0.5), 0 0 0 30px rgba(111,138,32, 0.5), 0 0 0 45px rgba(111,138,32, 0.5), 0 0 0 60px rgba(111,138,32, 0.5), 0 0 0 75px rgba(111,138,32, 0.5), 0 0 0 90px rgba(111,138,32, 0.5);
		}
		50% {
			box-shadow: 0 0 0 25px rgba(111,138,32, 0.5), 0 0 0 70px rgba(111,138,32, 0.5), 0 0 0 120px rgba(111,138,32, 0.5), 0 0 0 150px rgba(111,138,32, 0.5), 0 0 0 190px rgba(111,138,32, 0.5), 0 0 0 240px rgba(111,138,32, 0.5);
		}
		100% {
			box-shadow: 0 0 0 15px rgba(111,138,32, 0.5), 0 0 0 30px rgba(111,138,32, 0.5), 0 0 0 45px rgba(111,138,32, 0.5), 0 0 0 60px rgba(111,138,32, 0.5), 0 0 0 75px rgba(111,138,32, 0.5), 0 0 0 90px rgba(111,138,32, 0.5);
		}
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>