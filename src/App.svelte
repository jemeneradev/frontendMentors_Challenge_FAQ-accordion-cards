<script>
  import Card from "./Card.svelte";
</script>

<style>
  main {
    width: 327px;
    margin: 0;
  }

  @media screen and (min-width: 1440px) {
    main {
      width: 920px;
      margin-top: 100px;
    }
  }

  .design {
    position: absolute;
    margin: 0 auto;
    margin-top: -683px;
    margin-left: -8px;
    z-index: -10;
    /*  background-color: red; */
  }
  .design img {
    margin: 0 auto;
  }

  @media screen and (min-width: 1440px) {
    .design {
      margin-top: -638px;
    }
  }
</style>

<main>
  <Card />

  <div class="design">
    <picture>
      <source media="(min-width:1440px)" srcset="./design/desktop-design.jpg" />
      <source media="(max-width:1439px)" srcset="./design/mobile-design.jpg" />
      <img src="./design/mobile-design.jpg" alt="Mobile Design" />
    </picture>
  </div>
</main>
