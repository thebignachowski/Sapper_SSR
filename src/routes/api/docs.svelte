<script lang="ts">
  import { goto } from "@sapper/app";

  const goToHome = async () => {
    await goto(".", {
      replaceState: true,
    });
  };
</script>

<svelte:head>
  <title>Documentacion</title>
</svelte:head>

<h2>Documentación del API</h2>
<button on:click={goToHome}>Go to Home</button>
