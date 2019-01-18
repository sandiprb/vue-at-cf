<template>
  <div>
  <h1 class="home">Hello {{app}}</h1>
  <!-- <h2>{{sayMyName}}</h2> -->
  <!-- <a href="https://twitter.com/thepracticaldev/status/715623065078644738">JS</a> -->

  <input type="text" placeholder="Edit me" v-model="someInput">
  <h1>{{someInput}}</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "home",
  components: {
    HelloWorld
  },
  data: () => ({
    app: "Vue",
    fName: 'Sandip',
    lName: 'Baradiya',
    someInput: 'EDIT ME!',
  }),
  computed: {
    sayMyName(){
      return `${this.fName} ${this.lName}`
    }
  }
};
</script>
