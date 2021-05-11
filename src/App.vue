<template>
  <h1>Hello {{name}}</h1>
  <!-- <div v-text="channel"></div> -->
  <!-- <div v-html="color"></div> -->
  <!-- <h1 v-bind:id="headingID">Heading</h1> -->
  <button v-bind:disabled="idDisabled">Go More</button>
  <h1 class="underline">Another one</h1>
  <h1 v-bind:class="status">Status</h1>
  <h1 v-bind:class="soldOut">New Movie</h1>


</template>

<script>


export default {
  name: 'App',
  data () {
    return {
      name: 'Joshua',
      channel: 'NTV',
      color: '<h2>Blue</h2>',
      headingID: 'heading',
      idDisabled: false,
      status: 'danger',
      new: true,
      soldOut: true,
      idPromoted: true
    }
  }
  // components: {
  //   HelloWorld
  // }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.underline {
    text-decoration: underline;
  }

.danger, .soldOut{
  color: red;
}

.success, .isPromoted{
  color: green;
}

.new{
  text-decoration: italic;
}

</style>
