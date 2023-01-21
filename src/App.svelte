<script>
  import Header from "./UI/Header.svelte";
  import Content from "./UI/Content.svelte";
  import Footer from "./UI/Footer.svelte";
</script>

<style>
.container{
  height: 625.9px;
  margin: 1rem 6rem;

}
@media(max-width: 698px){
  .container{
    margin: 0;
  }
}
</style>

<main class="container">
  <Header />
  <Content />
  <Footer />
</main>