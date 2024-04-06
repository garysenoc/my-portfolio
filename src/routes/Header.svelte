<script>
	// @ts-ignore
	import { page } from '$app/stores';
	// @ts-ignore
	import logo from '$lib/images/svelte-logo.svg';
	// @ts-ignore
	import github from '$lib/images/github.svg';
  
	import "./app.css";
  
	function toggleMenu() {
	  const navContent = document.getElementById("nav-content");
	  // @ts-ignore
	  navContent.classList.toggle("hidden");
	  // @ts-ignore
	  navContent.classList.toggle("float-right");
	}
  </script>
  
  <link href="https://afeld.github.io/emoji-css/emoji.css" rel="stylesheet"> 
  <nav class="relative flex items-center justify-between flex-wrap bg-grey-darkest p-10 fixed w-full z-10 pin-t">
	<div class="flex items-center flex-no-shrink mr-6">
	  <a class="no-underline hover:no-underline" href="#">
		<span class="text-2xl pl-2"> garylloydsenoc</span>
	  </a>
	</div>
  
	<div class="block lg:hidden">
	  <button id="nav-toggle" on:click={toggleMenu} class="flex items-center px-3 py-2 border rounded text-grey border-grey-dark hover:text-white hover:border-white">
		<svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
	  </button>
	</div>
  
	<div class="w-full flex-grow lg:flex lg:items-center lg:w-auto hidden lg:block pt-6 lg:pt-0 lg:justify-end" id="nav-content">
		<ul class="list-reset lg:flex justify-end flex-1 items-center  float-end">
		  <li class="mr-3">
			<a class="inline-block text-grey-dark no-underline hover:text-grey-lighter hover:text-underline py-2 px-4" href="#">01. Blog</a>
		  </li>
		  <li class="mr-3">
			<a class="inline-block text-grey-dark no-underline hover:text-grey-lighter hover:text-underline py-2 px-4" href="#">02. Events</a>
		  </li>
		  <li class="mr-3">
			<a class="inline-block text-grey-dark no-underline hover:text-grey-lighter hover:text-underline py-2 px-4" href="#">03. Projects</a>
		  </li>
		  <li class="mr-3">
			<a class="inline-block text-grey-dark no-underline hover:text-grey-lighter hover:text-underline py-2 px-4" href="#">04. About</a>
		  </li>
		</ul>
	  </div>
  </nav>
  