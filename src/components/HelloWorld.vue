<template>
  <div class="hello">
    <a href="/">
      <div class="bg-primary text-white logo-nav-bar">
        <div class="container">
          <img
            class="logo-image"
            src="@/assets/Red-car-on-transparent-background-PNG.png"
            alt=""
          />
          Rent A Car
        </div>
      </div></a
    >
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.logo-image {
  width: 100px;
}

.logo-nav-bar {
  padding: 15px 0;
}
</style>
