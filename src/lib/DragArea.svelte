<script>
    export let id = '';
</script>
<style>
    .drag-area {
        width: 33.333%;
        height: 100vh;
    }

    #todo-area {
        background-color: lightgray;
    }

    #doing-area {
        background-color: darkgray;
    }

    #done-area {
        background-color: gray;
    }
</style>
<div class="drag-area" id="{id}">
    <slot></slot>
</div>