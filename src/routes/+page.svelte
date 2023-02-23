<style>
    .container {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
    }
</style>
<script lang="ts">
        import Item from '../lib/Item.svelte';
        import DragArea from '../lib/DragArea.svelte';
</script>
<div class="container">
    <DragArea id="todo-area">
        <Item/>
    </DragArea>
    <DragArea id="doing-area">
        <Item/>
    </DragArea>
    <DragArea id="done-area">
        <Item/>
    </DragArea>
</div>