<template>
  <section class="container">
    <h1>{{ title }}</h1>
    <p>{{ message }}</p>
    <hr>
    <router-link to="/">Go to Top</router-link>
  </section>
</template>

<script>
export default {
  data: function() {
    return {
      title: 'Other',
      message: 'これは、別ページです',
    };
  },
}
</script>