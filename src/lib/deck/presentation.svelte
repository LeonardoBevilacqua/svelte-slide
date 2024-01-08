<script lang="ts">
	// import Code from './code.svelte';
	import Markdown from './markdown.svelte';
	// import Slide from './slide.svelte';
</script>

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
