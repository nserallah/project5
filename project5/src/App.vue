<template>
  <div id="app">
    <nested-slot>
      <div slot="parent-slot">hello I am parent slot
        <div slot="child-slot">Hello I am child slot
          <p slot="grand-child-slot">Hello I am grandchild slot</p>
          <br><br>
        </div>
      </div>
      
      <template v-slot:slot1>  
        <h1>Hello I am came from NestedHead component</h1> 
      </template>
      <template v-slot:slot2>
        <p>Hello I am came from NestedHead component</p>
      </template>
    </nested-slot>

  </div>
</template>
<style scoped>
  
</style>
<script>

export default {
 data: function () {
    return {

    }
  },
  methods: {
    
  }
  
  
  
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  padding: 0;
  margin: 0;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
