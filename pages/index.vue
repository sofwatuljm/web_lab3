<template>
  <div class="container-fuild">
    <!--Halaman Background-->
    <div>
      <div class="hero">
        <h1>Selamat Datang Di Website SMKN 4 Tasikmalaya</h1>
      </div>
    </div>

    <div class="container">
      <h3 class="text-center mt-5">Sambutan Kepala Sekolah</h3>
      <div class="row clearfix">
        <img class="col-md-4" src="assets/img/kepalasekolah.jpg" alt="..." style="width: 20rem" />
        <p class="col-md-8 float-md-end mb-3">
          Assalamualaikum Warahmatullahi Wabarakatuh Selamat datang di SMKN 4 Tasikmalaya. Segala puji dan syukur kita panjatkan kehadirat Allah SWT, semoga kita semua ada dalam lindungan-Nya. Dan atas perkenan-Nya pula kami dapat
          menghadirkan website SMK Negeri 4 Tasikmalaya ini. Kami berharap dengan adanya website di SMK Negeri 4 Tasikmalaya ini para pengunjung dapat mengenal lebih jauh tentang sekolah kami sehingga dapat mempererat tali silaturrahmi
          antara sekolah dengan masyarakat demi kemajuan kita bersama. Tiada gading yang tak retak, website kami ini masih dalam proses pengembangan, masih banyak kekurangan yang harus kami perbaiki. Kritik dan sarannya yang membangun
          sangat kami harapkan untuk pengembangan ke depan. Akhirnya, saya mengucapkan terimakasih yang sebesar-besarnya kepada semua pihak yang tidak dapat disebutkan satu segala bantuan dan persatu atas fasilitasnya yang telah diberikan
          semoga semua yang kita lakukan bermanfaat bagi masyarakat. Wassalamu'alaikum Warahmatullahi Wabarakatuh.
        </p>
      </div>
    </div>

    <div class="container">
      <h3 class="text-center mb-5">Data Statistik</h3>
      <div class="row my-5 ms-5 text-dark">
        <div class="col-lg-3">
          <div class="card bg-light" style="height: 10rem">
            <div class="card-body">
              <h4 class="card-title text-md-center mt-5 fw-bold">80 Guru</h4>
            </div>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="card bg-light" style="height: 10rem">
            <div class="card-body">
              <h4 class="card-title text-md-center mt-5 fw-bold">1500 Siswa</h4>
            </div>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="card bg-light" style="height: 10rem">
            <div class="card-body">
              <h4 class="card-title text-md-center mt-5 fw-bold">10 Administrasi</h4>
            </div>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="card bg-light" style="height: 10rem">
            <div class="card-body">
              <h4 class="card-title text-md-center mt-5 fw-bold">18 Ekstrakurikuler</h4>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container">
      <h3 class="text-center mb-5">Kompetensi Keahlian</h3>
      <div class="row my-5">
        <!-- PPLG -->
        <div class="row align-items-center mb-4 justify-content-center">
          <div class="col-md-2 text-center">
            <img src="assets/img/rpl.jpg" alt="PPLG" class="img-fluid rounded" />
          </div>
          <div class="col-md-6">
            <h5 class="card-title text-center text-md-start">Pengembangan Perangkat Lunak Dan Gim (PPLG)</h5>
          </div>
        </div>

        <!-- TJKT -->
        <div class="row align-items-center mb-4 justify-content-center">
          <div class="col-md-2 text-center">
            <img src="assets/img/tjkt.jpg" alt="TJKT" class="img-fluid rounded" />
          </div>
          <div class="col-md-6">
            <h5 class="card-title text-center text-md-start">Teknik Jaringan Komputer Dan Telekomunikasi</h5>
          </div>
        </div>

        <!-- TBSM -->
        <div class="row align-items-center mb-4 justify-content-center">
          <div class="col-md-2 text-center">
            <img src="assets/img/tbsm.jpg" alt="TBSM" class="img-fluid rounded" />
          </div>
          <div class="col-md-6">
            <h5 class="card-title text-center text-md-start">Teknik Dan Bisnis Sepeda Motor</h5>
          </div>
        </div>

        <!-- DKV -->
        <div class="row align-items-center mb-4 justify-content-center">
          <div class="col-md-2 text-center">
            <img src="assets/img/dkv.jpg" alt="TBSM" class="img-fluid rounded" />
          </div>
          <div class="col-md-6">
            <h5 class="card-title text-center text-md-start">Desain Komunikasi Komputer</h5>
          </div>
        </div>

        <!-- TOI -->
        <div class="row align-items-center mb-4 justify-content-center">
          <div class="col-md-2 text-center">
            <img src="assets/img/toi.jpg" alt="TOI" class="img-fluid rounded" />
          </div>
          <div class="col-md-6">
            <h5 class="card-title text-center text-md-start">Teknik Otomasi Industri</h5>
          </div>
        </div>
      </div>
    </div>

    <div class="container">
      <h3 class="text-center pb-5">Berita</h3>
      <div class="row">
        <div v-for="(berita, i) in cover" :key="i" class="col-lg-4">
          <div class="card" style="width: 18rem">
            <img :src="berita.foto" class="card-img-top" />
            <div class="card-body">
              <h5 class="card-title">
                {{ berita.judul }}
              </h5>
              <p class="card-text">
                {{ berita.nama }}
              </p>
              <a href="https://radartasik.id/2024/05/21/ahm-resmikan-safety-riding-lab-di-smkn-4-tasikmalaya-wujudkan-komitmen-keselamatan-berkendara/" class="btn btn-primary">Selengkapnya</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!--Cards-->

  <!--Jurusan-->

  <!--Berita-->
</template>

<style scoped>
.hero {
  background-image: url("assets/img/smk4.JPG");
  height: 100vh;
  width: 100vw;
  color: white;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

<script setup>
useHead({
  title: "Beranda",
  meta: [
    {
      name: "description",
      content: "Beranda",
    },
  ],
});
const supabase = useSupabaseClient();
const cover = ref([]);

const getData = async () => {
  const { data, error } = await supabase.from("berita").select(`*`);
  if (data) cover.value = data;
};

onMounted(() => {
  getData();
});
</script>
