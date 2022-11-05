<template>
  <div id="app">
    
    <BaseLayout>
      <div slot="header">
        <h1>Hello from GumiHo</h1>
      </div>
      <div slot="main">
        <h3>Hello from Ronaldo</h3>
      </div>
      <div slot="footer">
        <h2>Hello from Messi</h2>
      </div>
      
    </BaseLayout>
  
  </div>
</template>

<script>
  import BaseLayout from './components/BaseLayout_Slot.vue'

export default {
 
  name: 'App',
  components: { 
    BaseLayout

  }
}

</script>

<style>

</style>
