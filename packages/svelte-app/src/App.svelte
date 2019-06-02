<script>
	import { Button } from "lib-with-bind-this";
	import ButtonFromPath from "../../lib-with-bind-this/src/Button.svelte";
	import LocalButton from "./LocalButton.svelte";
</script>

<style>

</style>

<h1>Svelte tests for bind:this</h1>

<p>The code for each button is identical, so each button should behave identically.</p>

<p><code>bind:this</code> only seems to work when the code is located in the same module as the app code.</p>

<p>For more details, open developer tools and click each button.</p>


<h2>Button from lib, esm import</h2>

<Button label="Button" />

<h2>Button from path</h2>

<ButtonFromPath label="Button" />

<h2>Local button</h2>

<LocalButton label="Button" />
