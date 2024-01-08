<script lang="ts">
	import Code from './code.svelte';
	import Slide from './slide.svelte';
</script>

<Slide animate>
	<Code lines id="code">
		{`
        function love() {}
        `}
	</Code>
</Slide>
<Slide animate>
	<Code lines id="code">
		{`
        function love() {
            console.log('Svelte')
        }
        `}
	</Code>
</Slide>

<Slide animate>
	<p class="uppercase">Transitions</p>
	<div class="flex place-content-center gap-2">
		<div data-id="box-1" class="h-[100px] w-[100px] bg-gray-400"></div>
		<div data-id="box-2" class="h-[100px] w-[100px] bg-gray-400"></div>
		<div data-id="box-3" class="h-[100px] w-[100px] bg-gray-400"></div>
	</div>
</Slide>

<Slide animate>
	<p class="uppercase">Transitions</p>
	<div class="flex place-content-center gap-2">
		<div data-id="box-1" class="h-[200px] w-[200px] bg-red-400"></div>
		<div data-id="box-2" class="h-[200px] w-[200px] bg-green-400"></div>
		<div data-id="box-3" class="h-[200px] w-[200px] bg-blue-400"></div>
	</div>
</Slide>
