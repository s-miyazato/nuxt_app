<template>
  <section class="container">
    <h1>{{ title }}</h1>
    <p>{{ message }}</p>
    <hr>
    <router-link to="/other">Go to Other</router-link>
  </section>
</template>

<script>
export default {
  data: function() {
    return {
      title: 'Hello',
      message: 'this is message.',
      now: 'wait...',
    };
  },

  created: function() {
    setInterval(()=> {
      let d = new Date();
      this.now = d.getHours()
      + ':' + d.getMinutes()
      + ':' + d.getSeconds();
    }, 1000);
  },
};
</script>

<style>
  .container {
    padding: 5px 10px;
  }
  h1 {
    font-size: 60pt;
  }
  p {
    padding-top: 5px;
  }
  hr {
    margin: 10px 0;
  }
</style>