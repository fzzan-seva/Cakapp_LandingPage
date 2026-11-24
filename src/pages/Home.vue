<template>
  <main id="top">
    <div class="w hero">
      <div>
        <div class="eb">Chat · Thread · Tugas</div>
        <h1>Chat lebih terarah,<br><mark>kerja lebih mudah</mark>.</h1>
        <p class="sub">Satu aplikasi untuk ngobrol dan mengatur pekerjaan tim.</p>
        <div class="cta-r">
          <a class="btn" href="#gabung">Coba Gratis</a>
          <a class="btn gh" href="#thread">Lihat Thread</a>
        </div>
      </div>
      <div class="stack">
        <span class="chip g" style="right:2%;top:10%">+ Jadikan tugas</span>
        <span class="chip w" style="left:0;bottom:12%;animation-delay:-3s">3 balasan</span>
        <div class="ph"><img src="/v7-daftar-obrolan-cak.app.png" alt="Daftar obrolan Cak.app"></div>
        <div class="ph c"><img src="/v7-ruang-obrolan-dengan-tombol-3-balasan.png" alt="Ruang obrolan dengan tombol 3 balasan"></div>
        <div class="ph"><img src="/v7-daftar-tugas-cak.app.png" alt="Daftar tugas Cak.app"></div>
      </div>
    </div>

    <section class="th" id="thread">
      <div class="w">
        <div>
          <span class="tag"><i></i>Thread</span>
          <h2>Satu pesan, satu ruang diskusi.</h2>
          <p class="sub">Obrolan utama tetap rapi.</p>
        </div>
        <div class="flow">
          <div class="fx">
            <span class="lb" style="left:50%;top:-14px;transform:translateX(-50%)">Ketuk 3 balasan</span>
            <div class="ph"><img src="/v7-ruang-obrolan-dengan-tombol-3-balasan.png" alt="Ruang obrolan dengan tombol 3 balasan"><div class="ring"></div></div>
          </div>
          <svg class="ar" viewBox="0 0 24 24" fill="none" stroke="#162136" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M4 12h16"/><path d="m14 6 6 6-6 6"/></svg>
          <div class="fx">
            <span class="lb" style="left:50%;top:-14px;transform:translateX(-50%)">Diskusi di sini</span>
            <div class="ph"><img src="/v7-layar-thread-cak.app.png" alt="Layar thread Cak.app"></div>
          </div>
        </div>
      </div>
    </section>

    <section class="st" id="tugas">
      <div class="w">
        <h2>Dari obrolan sampai tugas selesai.</h2>
        <div class="pair">
          <figure><div class="ph"><img src="/v7-daftar-obrolan-cak.app.png" alt="Daftar obrolan Cak.app"></div><figcaption>Obrolan</figcaption></figure>
          <figure style="margin-top:48px"><div class="ph"><img src="/v7-daftar-tugas-cak.app.png" alt="Daftar tugas Cak.app"></div><figcaption>Tugas</figcaption></figure>
        </div>
      </div>
    </section>

    <section class="cta" id="gabung">
      <img src="/v7-logo-cak.app.png" alt="Logo Cak.app"><h2>Coba Cak.app sekarang.</h2><a class="btn dk" href="#">Coba Gratis</a>
    </section>
  </main>
</template>

<script setup>
import { onMounted } from 'vue'
onMounted(() => {
  // language toggle handled in App.vue
})
</script>