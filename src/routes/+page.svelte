<script>
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Dropify" />
</svelte:head>

<main class="h-dvh p-8  w-full bg-zinc-500 size-12">
	<div class="h-full w-full rounded-3xl bg-white overflow-hidden wrapper">
    <div class="sidebar flex bg-blue-400">
      <img src="logo.svg" alt="">
      <div class="flex-col">
        <div class="flex">
          
        </div>
      </div>
    </div>
    <div class="main bg-amber-400">
    </div>
  </div>
</main>

<style>
  .wrapper{
    display: grid;
    grid-template-columns: 1fr 4fr;
    grid-template-rows: 1fr;
    grid-template-areas: 
    "sidebar main";
    gap: 1rem;
  }

  .sidebar{
    grid-area: sidebar;
    /* background-color: var(--accent-color); */
  }
  .main{
    grid-area: main;
    /* background-color: var(--background-color); */
  }
</style>
