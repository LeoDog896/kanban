<style>
    .item-container {
        border: 1px solid black;
        width: 80%;
        margin: auto;
        padding: 1rem;
        background-color: skyblue;
    }

    /* apply a grab cursor when hovering */
    .item-container:hover {
        /* fallback if grab isn't supported */
        cursor: move;
        cursor: grab;
    }

    /* apply a grabbing cursor when dragging */
    .item-container:active {
        cursor: grabbing;
    }
</style>
<script lang="ts">
    import { draggable } from '@neodrag/svelte';
	import { element } from 'svelte/internal';
    import { onMount } from 'svelte';

    
    
</script>
<div use:draggable={{ bounds: 'body' }} id="item" class="item-container">
    Hello!
</div>