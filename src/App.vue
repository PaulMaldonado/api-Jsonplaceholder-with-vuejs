<template>
  <div id="app">
   <Navbar />
   <Photo />
  </div>
</template>

<script>
import Navbar from './components/Navbar';
import Photo from './components/Photo';

export default {
  name: 'App',
  components: {
    Navbar,
    Photo
  }
}
</script>

<style>

</style>
