<script>
  export let item  

  const toggleStatus = () => {
    console.log(item)
  }
  
</script>

<li on:click={toggleStatus}>{item}</li>