<script lang="ts">
import {fly} from 'svelte/transition'
let visible = false;
</script>

<button on:click={() => visible = !visible}>Toggle visibility</button>

{#if visible}
    <div transition:fly>Hello!</div>
{/if}