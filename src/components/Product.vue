<template>
  <li>
    <div class="flex flex-wrap">
      <div class="w-full lg:w-1/3">
        <img :src="fotoP" alt="image" />
        <div class="title-price">
          <p>Title: {{ titleP }}</p>
          <p>Price: {{ priceP }}</p>
        </div>
      </div>
    </div>
  </li>
</template>

<script>
export default {
  // eslint-disable-next-line
  name: "Product",
  props: ["fotoP", "idP", "titleP", "priceP"],
};
</script>

<style scoped>
.grid {
  display: grid;
  grid-template-columns: 100px auto;
  grid-template-rows: auto;
}
img {
  width: 100%;
}

li {
  /* width: 300px; */
}

.title-price {
  display: flex;
  justify-content: space-between;
}
</style>
