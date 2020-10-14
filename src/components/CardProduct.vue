<template>
  <div class="card shadow card-product">
    <img
      :src="path + product.gambar"
      class="card-img-top"
      :alt="product.nama"
    />
    <div class="card-body">
      <h5 class="card-title">{{ product.nama }}</h5>
      <p class="card-text">Harga : Rp. {{ product.harga }}</p>
      <router-link :to="'/foods/' + product.id" class="btn btn-success"
        ><b-icon-cart></b-icon-cart> Pesan</router-link
      >
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "CardProduct",
  props: ["product"],
  data() {
    return {
      path: axios.defaults.baseURL,
    };
  },
};
</script>
