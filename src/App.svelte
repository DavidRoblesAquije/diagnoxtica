<script>
  import viteLogo from "/vite.svg";
  import Cabezera from "./components/cabezera.svelte";
  import Nosotros from "./components/nosotros.svelte";
  import Servicios from "./components/servicios.svelte";
  import Opiniones from "./components/opiniones.svelte";
  import Sedes from "./components/sedes.svelte";
  import Footer from "./components/footer.svelte";
    import Enlacesfijos from "./components/enlacesfijos.svelte";
    import Navbar from "./template/navbar.svelte";
</script>

<main>
  <!-- Navegacion -->
  <Navbar/>
  <!-- enlaces fijos -->
  <Enlacesfijos />
  <!-- secciones -->
  <Cabezera />
  <Nosotros />
  <Servicios />
  <Opiniones />
  <Sedes />
  <Footer />
</main>
