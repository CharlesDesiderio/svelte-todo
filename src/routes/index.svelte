<script>
  let list = []
  let inputValue = ''

  const addToList = () => {
    list = [...list, inputValue]
    inputValue = ''
    console.log(list)
  }

  import Component from "./component.svelte";

</script>

<div>
<h1>To Do List</h1>
<input bind:value={inputValue}>
<button on:click={addToList}>Submit</button>
{#each list as listItem}
<Component item={listItem} />
{/each}


</div>