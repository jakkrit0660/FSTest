<template>
  <div>
    <h1>{{ title }}</h1>
    <input
      v-model="msg"
      type="text"
      id="text"
      placeholder="Type Something"
    /><br />
    <p>{{ text }}</p>
    <p>{{ msg }}</p>
  </div>
</template>
<script>
export default {
  name: 'myText',
  data () {
    return {
      title: 'Hello World',
      text: 'The Text will show down here',
      msg: ''
    }
  }
}
</script>
