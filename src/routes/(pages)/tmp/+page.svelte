<script>
	import { screenType, mouseOnLink } from '$lib/store/store';
	import { setMouseOnLink, setMouseOffLink } from '$lib/functions/mouse.js';
</script>

<section>
	<header>
		{#if $screenType == 3}
			<p>click to build / shift-click to demolish</p>
		{/if}
	</header>
	<div class="body">
		<!--img class="niels" alt="niels" src="/niels_bw.jpg" /-->

		<div class="grey top">
			<h1>aufbau.</h1>

			<div class="top__text">
				<p>CREATIVE // TECHNICAL</p>
				<p>ldn • ykt • nyc</p>
			</div>
		</div>

		<div class="grey body__left">
			<h3>work</h3>

			<!-- <a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				href="https://zen.aufbau.io"
				target="_blank"
				>zen • web art • 2021
			</a> -->

			<a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				href="https://iota.health"
				target="_blank"
				>iota • research app • WIP
			</a>

			<!-- <a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				href="https://www.conceptioncalculator2000.com"
				target="_blank"
				>conception calculator 2000 • web • WIP
			</a> -->
			<a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				href="https://replikamasterworks.com"
				target="_blank"
				>replika • website • WIP
			</a>
			<!-- <a href="https://site.hhacker.space" target="_blank">hedron hackerspace • web • 2022</a> -->
		</div>
		<div class="grey body__right">
			<h3>systems</h3>
			<a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				href="/systems">modular system architecture • example</a
			>
		</div>
		<div class="grey hidden body__left">
			<p>bespoke websites, systems, apps</p>
			<p>microservice, and 3d specialist</p>
		</div>
		<div class="body__right">
			<h3>say hi</h3>

			<a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				target="_blank"
				href="https://github.com/aufbau-io">github</a
			>
			<a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				href="mailto: dan@aufbau.io">email</a
			>
			<a
				on:mouseenter={() => setMouseOnLink()}
				on:mouseleave={() => setMouseOffLink()}
				class="hide"
				target="_blank"
				href="/dan_humphries_cv.pdf">cv</a
			>
		</div>
		<br />
	</div>
	<footer>
		<a
			on:mouseenter={() => setMouseOnLink()}
			on:mouseleave={() => setMouseOffLink()}
			href="https://www.websitecarbon.com/website/aufbau-io/">0.04g of CO2 / visit</a
		>
	</footer>
</section>

<style>
	section {
		height: 100vh;
		height: calc(var(--vh, 1vh) * 100);
		display: flex;
		overflow: auto;
		max-width: 640px;
		touch-action: manipulation;
	}

	.body {
		position: relative;
		margin: auto 0;
		display: flex;
		flex-flow: column nowrap;
		justify-content: center;
		background: var(--background-50);
		border: solid 1px var(--primary-50);
		border-radius: 16px;
		padding: 40px;
	}

	.grey {
		margin: 16px 0;
	}

	.grey.top {
		margin-bottom: 0;
		padding-bottom: 16px;
		margin-top: 0;
		display: flex;
		justify-content: space-between;

		border-bottom: solid 1px var(--primary-50);
	}

	.top__text {
		display: flex;
		flex-flow: column wrap;
		justify-content: flex-end;
		align-items: flex-end;
	}

	.top__text p {
		text-align: right;
	}

	.body__left {
		text-align: left;
	}

	.body__right {
		text-align: right;
	}

	header {
		position: absolute;
		top: 24px;
		left: 0;
		width: 100vw;

		display: flex;
		justify-content: center;
	}

	footer {
		position: absolute;
		bottom: 24px;
		left: 0;
		width: 100vw;

		display: flex;
		justify-content: center;
	}

	footer a,
	header p {
		background: var(--background);
		color: var(--primary-50);
		border: solid 1px var(--primary-50);
	}

	footer a:hover {
		color: var(--accent);
		border: solid 1px var(--primary-50);
	}

	@media (max-width: 760px) {
		section {
			height: 94vh;
			height: calc(var(--vh, 1vh) * 94);
		}

		.grey {
			margin: 8px;
		}
		.body {
			padding: 16px 8px;
			margin: auto 16px;
		}
	}
</style>
