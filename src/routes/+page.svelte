<svelte:head>
  <title>RelaxGame</title>
</svelte:head>

<main class="page">
  <h1>Welcome to RelaxGame</h1>
  <p>A calming SvelteKit app ready for GitHub Pages deployment.</p>
  <button type="button">Start Breathing</button>
</main>

<style>
  .page {
    min-height: 100vh;
    display: grid;
    place-content: center;
    gap: 1rem;
    text-align: center;
    padding: 2rem;
  }

  h1 {
    margin: 0;
    color: #f5e3d1;
    font-size: clamp(1.6rem, 5vw, 2.4rem);
  }

  p {
    margin: 0;
    color: rgba(245, 227, 209, 0.85);
  }

  button {
    justify-self: center;
    border: 1px solid rgba(248, 230, 213, 0.4);
    background: rgba(255, 241, 226, 0.16);
    color: #f7e8d9;
    border-radius: 999px;
    padding: 0.6rem 1.2rem;
    cursor: pointer;
  }
</style>
