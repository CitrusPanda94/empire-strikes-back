<template>
  <div class="container">
    <h1>Detail</h1>
    <Content v-bind:contentdata="contentdata"/>
  </div>
</template>

<script>
  export default {
    name: "Content",
    props: ["data"],
    watch: {
      data: function(val) {
        this.data=val;
      }
    }
  }
  
</script>
<!-- <h2>{{ data.name }}</h2> -->

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.info h2, p {
  text-align: left;
  margin-bottom: 20px;
}
  
</style>