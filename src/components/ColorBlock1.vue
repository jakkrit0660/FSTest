<template>
  <div>
      <li>
      <p style='width: 200px; height: 200px;' v-bind:style="{'background-color': bgColor1}">{{bgColor1}}</p>
      </li>
  </div>
</template>
<script>
export default {
  name: 'ColorBlock1',
  props: [ 'bgColor1' ],
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
