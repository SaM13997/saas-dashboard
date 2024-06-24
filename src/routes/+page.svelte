<script lang="ts">
	import Icon from '@iconify/svelte'
	import { fade } from 'svelte/transition'
	import SidebarItem from '../components/SidebarItem.svelte'
  import BarChart from '../components/BarChart.svelte'
</script>
<svelte:head>
	<title>Home</title>
	<meta name="description" content="Dropify" />
</svelte:head>

<main class="h-dvh p-8 w-full bg-zinc-500 size-12">
	<div class="h-full w-full rounded-3xl bg-white overflow-hidden wrapper">
		<div class="sidebar flex flex-col p-6 pr-0 justify-between">
			<div class="flex flex-col gap-6">
				<div class="flex items-center pl-1 gap-2">
					<Icon
						icon="arcticons:hex"
						class="text-5xl text-[var(--accent-color)] stroke-[3]"
					/>
					<p class="text-4xl text-[var(--background-color)]">Dropify</p>
				</div>
				<div class=" flex flex-col gap-2 w-full">
					<SidebarItem itemName="Dashboard" itemIcon="iconamoon:home" />
					<SidebarItem itemName="Orders" itemIcon="iconoir:truck" />
					<SidebarItem
						itemName="Shipments"
						itemIcon="teenyicons:curved-connector-outline"
					/>
					<SidebarItem
						itemName="Map Overview"
						itemIcon="mingcute:world-2-line"
					/>
					<SidebarItem
						itemName="Messages"
						itemIcon="iconoir:mail"
						additionalData="2"
					/>
					<SidebarItem itemName="Settings" itemIcon="tdesign:setting" />
				</div>
			</div>
			<div class="controls flex flex-col">
				<div class="flex gap-2 items-center">
					<img
						class="size-12"
						src="https://avatar.iran.liara.run/public/47"
						alt=""
					/>
					<div class="flex flex-col justify-between text-zinc-900">
						<p class="text-xl">Sam Byrd</p>
						<p class="text-zinc-600 text-xs">Toronto,ON</p>
					</div>
					<Icon
						class="text-2xl text-zinc-600 ml-auto"
						icon="ic:baseline-logout"
					/>
				</div>
			</div>
		</div>
		<div class="main flex flex-col p-6 gap-8 pl-0">
			<div class="header flex justify-between items-center">
				<div class="flex flex-col">
					<p class="text-xl font-semibold text-[var(--background-color)]">
						Welcome Back, Sam!
					</p>
					<p class="text-xs text-zinc-500">You have one unprocessed order</p>
				</div>
				<div class="flex gap-4">
					<div
						class="size-10 flex justify-center items-center aspect-square bg-zinc-800 text-zinc-200 rounded-full shadow"
					>
						<Icon icon="ph:bell-bold" />
					</div>
					<div
						class="size-10 flex justify-center items-center aspect-square bg-zinc-800 text-zinc-200 rounded-full shadow"
					>
						<Icon class="text-xl" icon="ic:baseline-search" />
					</div>
					<div
						class="size-10 flex justify-center items-center aspect-square bg-zinc-800 text-zinc-200 rounded-full shadow"
					>
						<Icon class="text-xl" icon="mynaui:message" />
					</div>
					<div
						class="h-10 w-max flex justify-center items-center px-4 text-sm font-semibold bg-[var(--accent-color)] text-zinc-100 rounded-full shadow"
					>
						Create New Order
					</div>
				</div>
			</div>
			<div class="second-row gap-4 flex w-full justify-between">
				<!-- <div class="flex w-1/3 max-h-36 p-4 bg-zinc-100 gap-4 rounded-3xl">
					<div class="flex flex-col w-1/2 overflow-hidden justify-between gap-2">
						<p
							class="text-[var(--background-color)] text-2xl w-max font-semibold"
						>
							This month's orders
						</p>
						<div class="flex gap-2 items-end">
							<div
								class="size-14 flex justify-center items-center aspect-square bg-zinc-800 text-zinc-200 rounded-full shadow"
							>
								<Icon class="text-3xl" icon="ic:baseline-search" />
							</div>
							<p class="text-4xl text-[var(--background-color)]">132</p>
							<p class="text-xs text-[var(--accent-color)] mb-1">+25%</p>
						</div>
					</div>
					<BarChart />
				</div> -->
				<div class="flex max-h-36 p-4 bg-zinc-100 gap-4 rounded-3xl">
					<div class="flex flex-col justify-between gap-2">
						<p
							class="text-[var(--background-color)] text-2xl w-max font-semibold"
						>
							This month's orders
						</p>
						<div class="flex gap-2 items-end">
							<div
								class="size-14 flex justify-center items-center aspect-square bg-zinc-800 text-zinc-200 rounded-full shadow"
							>
								<Icon class="text-3xl" icon="ic:baseline-search" />
							</div>
							<p class="text-4xl text-[var(--background-color)]">132</p>
							<p class="text-xs text-[var(--accent-color)] mb-1">+25%</p>
						</div>
					</div>
					<BarChart />
				</div>
				<div class="flex max-h-36 p-4 bg-zinc-100 gap-4 rounded-3xl">
					<div class="flex flex-col justify-between gap-2">
						<p
							class="text-[var(--background-color)] text-2xl w-max font-semibold"
						>
							This month's orders
						</p>
						<div class="flex gap-2 items-end">
							<div
								class="size-14 flex justify-center items-center aspect-square bg-zinc-800 text-zinc-200 rounded-full shadow"
							>
								<Icon class="text-3xl" icon="ic:baseline-search" />
							</div>
							<p class="text-4xl text-[var(--background-color)]">132</p>
							<p class="text-xs text-[var(--accent-color)] mb-1">+25%</p>
						</div>
					</div>
					<BarChart />
				</div>
				<div class="flex max-h-36 p-4 bg-zinc-100 gap-4 rounded-3xl">
					<div class="flex flex-col justify-between gap-2">
						<p
							class="text-[var(--background-color)] text-2xl w-max font-semibold"
						>
							This month's orders
						</p>
						<div class="flex gap-2 items-end">
							<div
								class="size-14 flex justify-center items-center aspect-square bg-zinc-800 text-zinc-200 rounded-full shadow"
							>
								<Icon class="text-3xl" icon="ic:baseline-search" />
							</div>
							<p class="text-4xl text-[var(--background-color)]">132</p>
							<p class="text-xs text-[var(--accent-color)] mb-1">+25%</p>
						</div>
					</div>
					<BarChart />
				</div>
			</div>
		</div>
	</div>
</main>

<style>
	
	.wrapper {
		display: grid;
		grid-template-columns: 1fr 5fr;
		grid-template-rows: 1fr;
		grid-template-areas: 'sidebar main';
		gap: 1rem;
	}

	.sidebar {
		grid-area: sidebar;
		/* background-color: var(--accent-color); */
	}
	.main {
		grid-area: main;
		/* background-color: var(--background-color); */
	}
</style>
