<template>
  <div class="container pt-5 pb-5 mb-5">
    <div class="row">
      <form>
        <div class="mb-3">
          <label for="exampleInputtext" class="form-label">Nama</label>
          <input type="text" class="form-control" id="exampleInputtext" />
        </div>
        <div class="mb-3">
          <label for="exampleInputEmail1" class="form-label">Email</label>
          <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" />
          <div id="emailHelp" class="form-text"></div>
        </div>

        <div class="mb-3">
          <label for="exampleInputtext" class="form-label">Pesan</label>
          <textarea class="form-control" style="height: 100px"></textarea>
        </div>
        <button type="submit" class="btn btn-primary">Kirim</button>
      </form>
    </div>
  </div>
</template>

<script setup>
useHead({
  title: "Kontak",
  meta: [
    {
      name: "description",
      content: "Kontak",
    },
  ],
});
</script>
