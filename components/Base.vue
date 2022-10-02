<!-- Please remove this file from your project -->
<template>
  <main>
    <Navbar />
    <Header />
    <Brands />
    <Experience />
    <BespokeSolution />
  </main>
</template>

<script>
import Navbar from "./Layouts/Navbar.vue";
import BespokeSolution from "./Bespoke-solution.vue";

export default {
  name: "Index",
  components: { Navbar, BespokeSolution },
};
</script>
<style></style>
