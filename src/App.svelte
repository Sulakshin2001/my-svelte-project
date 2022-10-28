
<script>
  import Loader1 from "./components/loaders/Loader1.svelte";
  import Loader2 from "./components/loaders/Loader2.svelte";

  let timer = 0
  function change() {
      timer=1
  }
  setTimeout(change,10000)
</script>
{#if timer===0}
    <Loader1/>
    {/if}
{#if timer===1}
    <Loader2/>
{/if}