<style>
    .container {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
    }

    .drag-area {
        width: 30%;
        height: 100vh;
        border-left: 1px solid black;
        border-right: 1px solid black;
    }
</style>
<script lang="ts">
        import Item from '../lib/Item.svelte';
        import { onMount } from 'svelte';
        onMount(() => {
            const item = document.getElementById('item') || new Element();
            item.addEventListener('onclick', ((event) => {
            //do something
            console.log(event);
            }) as EventListener);
    })
</script>
<div class="container">
    <div class="drag-area" >
        <Item/>
    </div>
    <div class="drag-area">

    </div>
    <div class="drag-area">

    </div>
</div>