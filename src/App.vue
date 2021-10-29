<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="https://vuejs.org/images/logo.png" /> -->
    <div class="inline" >
      {{ getname }}
    </div>
    <button @keyup.Enter="handlerClick">按钮p</button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {},
  data() {
    return {
      getname: '123',
    };
  },
  methods: {
    handlerClick() {
      if (this.getname != '123') {
        this.getname = '123';
      } else {
        this.getname = '222';
      }
    },
  },
};
</script>
<style>
.inline {

}
</style>