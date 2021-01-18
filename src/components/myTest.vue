<template>
  <body>
    <h1>Hello World</h1>
    Type Something: <input type="text" id="text" /><br />
    <button @click="showtext()">Click</button><br />
    <p>The text will show down here</p>
    <p id="line1"></p>
  </body>
</template>
<script>
export default {
  methods: {
    showtext() {
      var Stext = document.getElementById("text").value;
      document.getElementById("line1").innerHTML = Stext;
    },
  },
};
</script>
