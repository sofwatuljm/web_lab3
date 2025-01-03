<template>
  <diV class="container bg-secondary mt-5">
    <div class="row">
      <h3 class="text-center text-white">Pembukaan Masa Pengenalan Lingkungan Sekolah</h3>
      <p class="text-center text-white">Tahun Pelajaran 2023/2024</p>
      <div v-for="(galeri, i) in galeri" :key="i" class="col-lg-4">
        <div class="p-3 mb-5">
          <img :src="galeri.foto" class="card-img-top" />
          <div class="card-body">
            <h5 class="card-title">{{ galeri.nama }}</h5>
          </div>
        </div>
      </div>
    </div>
  </diV>
</template>
<script setup>
useHead({
  title: "Galeri",
  meta: [
    {
      name: "description",
      content: "Galeri",
    },
  ],
});
const supabase = useSupabaseClient();

const galeri = ref([]);

const getCover = async () => {
  const { data } = await supabase.from("galeri").select(`*`);
  if (data) galeri.value = data;
};

onMounted(() => {
  getCover();
});
</script>
