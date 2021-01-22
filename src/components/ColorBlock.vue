<template>
  <div>
      <ul>
          <li v-for="Cl in bgColor" v-bind:key="Cl" style="width: 200px; height: 200px;" v-bind:style="{'background-color': Cl.color}">{{Cl.color}}
          </li>
      </ul>
  </div>
</template>
<script>
export default {
  name: 'ColorBlock',
  props: [ 'bgColor' ],
}
</script>
<style>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
</style>
