<script>
  let bar = 'h-full w-[30px] rounded-t-lg bg-purple-200'
</script>

<div class="barChart min-w-1/2 gap-2">
	<div class="{bar}"></div>
	<div class="{bar}"></div>
	<div class="{bar}"></div>
	<div class="{bar}"></div>
	<div class="{bar}"></div>
	<p class="text-[10px] text-center">JUN</p>
	<p class="text-[10px] text-center ">JUL</p>
	<p class="text-[10px] text-center ">AUG</p>
	<p class="text-[10px] text-center  ">SEP</p>
	<p class="text-[10px] text-center ">OCT</p>
</div>

<style>
  .barChart {
		display: grid;
		grid-template-columns: repeat(5, minmax(30px, 1fr));
		grid-template-rows: 5fr 1fr;
	}
</style>