<template>
  <main>
    <h1>Easy Elevations</h1>
    <h4>The Top Man Assistant</h4>
    <div>
      <h1>Curret Jobs</h1>
      <h2 v-for="(project, index) in projects" 
      :key="index">{{ project.name }}</h2>
    </div>
  </main>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      projects: [
        {name: 'EcoStation', jobNumber: ''},
        {name: 'H2', jobNumber: ''},
        {name: 'Heritage', jobNumber: ''},
        {name: 'Orchards', jobNumber: ''}
      ]
    }
  },
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  text-align: center;
}
h2 {
  text-align: center;
}
h4 {
  text-align: center;
}
</style>
