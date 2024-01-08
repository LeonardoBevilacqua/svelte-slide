<script lang="ts">
	import Code from './code.svelte';
	import Markdown from './markdown.svelte';
	import Notes from './notes.svelte';
	import Slide from './slide.svelte';
</script>

<Slide>
	<h1>Exemple Slides</h1>

	<Notes>Notes 1</Notes>
</Slide>
<Slide>
	<h1>Slide 1</h1>

	Horizontal slide

	<Notes>Notes 2</Notes>
</Slide>
<Slide>
	<h1>Slide 2</h1>

	<Slide>Vertical slide 1</Slide>
	<Slide>Vertical slide 2</Slide>

	<Notes>Notes 3</Notes>
</Slide>
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
	<p class="uppercase text-red-300">Transitions</p>
	<div class="flex place-content-center gap-2">
		<div data-id="box-1" class="h-[200px] w-[200px] bg-red-400"></div>
		<div data-id="box-2" class="h-[200px] w-[200px] bg-green-400"></div>
		<div data-id="box-3" class="h-[200px] w-[200px] bg-blue-400"></div>
	</div>
</Slide>
<Markdown>
	{`
        \`\`\`js [1-2|3|4]
        let a = 1;
        let b = 2;
        let c = x => 1 + 2 + x;
        c(3);
        \`\`\`
    `}
</Markdown>
<Markdown name="exemple.md" external />
