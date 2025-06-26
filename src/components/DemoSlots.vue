<template>
  <h1>Demo Slots</h1>
  <header>
    <slot name="header"></slot>
  </header>
  <main>
    <section class="one">
        <slot></slot>
  </section>
  <section class="two">
        <slot></slot>
  </section>
  </main>
  
  <footer>
    <slot name="footer"></slot>
  </footer>
</template>

<script>
export default {

}
</script>

<style>

</style>