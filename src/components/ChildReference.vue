<template>
  <div class="child-reference">
    <h4>Child with reference as prop</h4>
    <p>Value of child:</p> 
    {{ valueReference }}
    <br>
    <br>
    Value cat: <input type="text"
          v-model="valueReference.cat">
    <br>
    Value dog:<input type="text"
          v-model="valueReference.dog">    

  </div>
</template>

<script>
export default {
  name: "ChildReference",
  props: {
    valueReference: Object
  },
  data() {
    return {};
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
