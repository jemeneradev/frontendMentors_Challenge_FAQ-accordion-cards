<script>
  import Card from "./Card.svelte";

  let showActive = false;
  let showDesign = true;
  let makeTransparent = true;
</script>

<style>
  main {
    
    display: flex;
    justify-content: center;
    align-items: center;
    /* margin: auto auto; */
  }

  @media screen and (min-width: 1440px) {
    main {
      width: 920px;
      /* margin-top: 100px; */
    }
  }

  .design {
    position: absolute;
    margin: 0 auto;
    top: 0;
    left: 0;
    z-index: -10;
    /*  background-color: red; */
  }
  .design img {
    margin: 0 auto;
  }
  .controls {
    position: absolute;
    bottom: 0px;
    width: 500px;
  }
  .controls ul {
    display: flex;
  }
  .controls ul li {
    list-style: none;
    display: inline;
    margin-left: 20px;
  }

  
  :global(body) {
    background:  linear-gradient(hsl(273, 75%, 66%), hsl(240, 73%, 65%));
  }
  
</style>

<!-- {#if showDesign === true}
  <div class="design">
    {#if showActive !== true}
      <picture>
        <source
          media="(min-width:1440px)"
          srcset="./design/desktop-design.jpg" />
        <source
          media="(max-width:1439px)"
          srcset="./design/mobile-design.jpg" />
        <img src="./design/mobile-design.jpg" alt="Mobile Design" />
      </picture>
    {:else}
      <picture>
        <source
          media="(min-width:1440px)"
          srcset="./design/active-states.jpg" />
        <source
          media="(max-width:1439px)"
          srcset="./design/mobile-active-state.jpg" />
        <img src="./design/active-states.jpg" alt="Mobile Design" />
      </picture>
    {/if}
  </div>
{/if} -->

<main>
  <Card />

  <!-- <div class="design">
    <picture>
      <source media="(min-width:1440px)" srcset="./design/desktop-design.jpg" />
      <source media="(max-width:1439px)" srcset="./design/mobile-design.jpg" />
      <img src="./design/mobile-design.jpg" alt="Mobile Design" />
    </picture>
  </div> -->
</main>

<!-- <div class="controls">
  <ul>
    <li>
      <label for="showDesign">Show Design</label>
      <input
        type="checkbox"
        id="design-show"
        bind:checked={showDesign}
        name="showDesign" />
    </li>

    <li>
      <label for="showActive">Show Active State</label>
      <input
        type="checkbox"
        id="active-show"
        bind:checked={showActive}
        name="showActive" />
    </li>
    <li>
      <label for="tranparent">Make Transparant</label>
      <input
        type="checkbox"
        id="active-show"
        bind:checked={makeTransparent}
        name="showActive" />
    </li>
  </ul>
</div> -->
