<template>
  <div class="pesanan">
    <Navbar />
    <div class="container">
      <div class="row justify-content-center mt-5">
        <div class="col text-center">
            <img src="../assets/images/cooking-wait.png" width="500" alt="waiting">
            <h2><strong>Sukses!!</strong></h2>
            <h4>Pesanan Anda segera diproses <br> Selamat Menunggu</h4>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";

export default {
  nama: "Pesanan",
  components: {
    Navbar,
  },
};
</script>

<style></style>
