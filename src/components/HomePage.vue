<template>
  <div>
    <Navbar></Navbar>
    <div class="container">
      <div class="product">
        <ul>
          <Product
            v-for="image in images"
            :key="image.id"
            :foto-p="image.photo"
            :id-p="image.id"
            :title-p="image.title"
            :price-p="image.price"
          ></Product>
        </ul>
      </div>
    </div>

    <Footer></Footer>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import Product from "./Product.vue";

export default {
  components: {
    Navbar,
    Footer,
    Product,
  },
  data() {
    return {
      images: [
        {
          id: 1,
          price: 1458,
          title: "Leopard",
          photo:
            "https://cdn.pixabay.com/photo/2021/11/11/13/08/leopard-6786267__340.jpg",
        },
        {
          id: 2,
          price: 1458,
          title: "Lion",
          photo:
            "https://cdn.pixabay.com/photo/2020/07/01/17/34/wolf-5360340__340.jpg",
        },
        {
          id: 3,
          price: 1458,
          title: "Tiger",
          photo:
            "https://cdn.pixabay.com/photo/2020/09/23/17/12/flowers-5596564__340.png",
        },
        {
          id: 4,
          price: 1458,
          title: "Kaplan",
          photo:
            "https://cdn.pixabay.com/photo/2021/10/27/08/43/forest-6746433__340.jpg",
        },
        {
          id: 5,
          price: 1458,
          photo:
            "https://cdn.pixabay.com/photo/2021/11/03/09/25/squirrel-6765124__340.jpg",
        },
        {
          id: 6,
          price: 1458,
          photo:
            "https://cdn.pixabay.com/photo/2021/05/09/06/07/dog-6240043__340.jpg",
        },
      ],
    };
  },
};
</script>

<style scoped>
ul {
  list-style: none;
  /* display: flex; */
  /* gap: 1rem; */
  /* flex-wrap: wrap; */
  padding: 0;
  /* justify-content: space-between; */
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, auto));
  gap: 2rem;
}
</style>
