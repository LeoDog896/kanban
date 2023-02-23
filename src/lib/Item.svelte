<style>
    .item-container {
        border: 1px solid black;
        width: 80%;
        margin: auto;
        padding: 1rem;
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
    import randomColor from 'randomcolor'; 
</script>
<div use:draggable={{ bounds: 'body' }} id="item" style="background-color: {randomColor({ luminosity: 'light' })}" class="item-container">
    Hello!
</div>