<template>
  <div>
    <h1>{{pageName}} Component</h1>
    <h1>{{ product.name }} {{product.platform}} - {{this.pageName}}</h1>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      product: {
        name: "MyJSQL",
        platform: "WebApp"
      },
      pageName: "Home"
    };
  }
};
</script>


<style>
h1 {
  color: slateblue;
}
</style>
