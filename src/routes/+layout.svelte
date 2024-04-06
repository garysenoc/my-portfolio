<script>
	import Header from './Header.svelte';
	import Footer from './Footer.svelte'
	import Profile from '../lib/images/profile.jpg';
	import './app.css';
</script>

<div class="app">
	<Header />
	<main >
		
		<!-- <enhanced:img src={Profile} alt="An alt text"/> -->
		<div class="flex flex-row justify-center">
			<div  class="min-w-[400px] min-h-[400px] w-[400px] max-w-[400px]">
				<img src={Profile} alt="An alt text" style={"border-radius: 20px"}/>
			</div>
		
				<div class="w-[600px] flex items-center ml-[60px]">
					<div class="flex-col">
						<p class="text-[20px]">👋 Hello! My name is</p>
						<h1 class="font-bold text-5xl">Gary Lloyd Senoc</h1>
						<br/>
						<br/>
						<p class="text-[20px]">Gary, a Cloud Engineer at Senti AI, a leading AI firm in the Philippines, holds a Bachelor of Science degree in Computer Science from Cebu Institute of Technology - University. His tech journey began with freelance work in high school and expanded through active participation in tech competitions, enriching his expertise in technology through collaborations with local and international companies. </p>
						
				</div>
				
		</div>
	
	</main>

	<Footer/>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 80rem;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>
