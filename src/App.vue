<template>
  <div style="background:#fff;position:sticky;top:0;z-index:10">
    <div style="max-width:1200px;margin:0 auto;padding:0 32px;box-sizing:border-box;height:76px;display:flex;align-items:center;gap:32px">
      <div style="display:flex;align-items:center;gap:12px">
        <img src="/v7-logo-cak.app.png" alt="Logo Cak.app" style="width:40px;height:40px;display:block">
        <b style="font-size:22px;color:#162136">Cak.app</b>
      </div>
      <div style="flex:1"></div>
      <a class="nv" href="#thread" style="color:#162136;font-size:16px">Fitur</a>
      <a class="nv" href="#perangkat" style="color:#162136;font-size:16px">Perangkat</a>
      <a class="nv" href="#paket" style="color:#162136;font-size:16px">Paket</a>
      <a class="nv" href="#bantuan" style="color:#162136;font-size:16px">Bantuan</a>
      <div class="lg">
        <button class="lg-b" id="lgb" type="button" aria-haspopup="listbox" aria-expanded="false" aria-controls="lgm" aria-label="Pilih bahasa">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle cx="12" cy="12" r="9"/><path d="M3 12h18"/><path d="M12 3a14 14 0 0 1 0 18a14 14 0 0 1 0-18"/></svg>
          <span id="lgl">ID</span>
          <svg class="ch" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="m6 9 6 6 6-6"/></svg>
        </button>
        <div class="lg-m" id="lgm" role="listbox" aria-label="Pilih bahasa">
          <small>Pilih bahasa</small>
          <button type="button" role="option" data-l="id" aria-selected="true">Bahasa Indonesia<svg class="ck" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#167a58" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="m5 12 5 5 9-10"/></svg></button>
          <button type="button" role="option" data-l="en" aria-selected="false">English<svg class="ck" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#167a58" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="m5 12 5 5 9-10"/></svg></button>
        </div>
      </div>
      <a href="#" style="color:#162136;font-size:16px;font-weight:600">Masuk</a>
      <button onclick="location.hash='gabung'" style="background:#a5bf98;color:#162136;border:0;border-radius:40px;padding:12px 24px;font-size:16px;font-weight:600;font-family:inherit;line-height:1.2">Coba Gratis</button>
    </div>
  </div>

  <nav class="mobile-nav">
    <a href="#thread">Fitur</a>
    <a href="#perangkat">Perangkat</a>
    <a href="#paket">Paket</a>
    <a href="#bantuan">Bantuan</a>
  </nav>

  <main id="top">
    <!-- Hero -->
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

    <!-- Thread / Fitur -->
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

    <!-- Fitur -->
    <section class="st" id="fitur">
      <div class="w">
        <h2>Fitur</h2>
        <p class="sub" style="margin:12px auto 0;max-width:640px">Satu aplikasi untuk ngobrol dan mengatur pekerjaan tim.</p>
        <div class="feature-grid">
          <div class="fc">
            <h3>Chat</h3>
            <p>Pribadi, divisi, dan proyek. Kirim pesan dan lampiran di satu tempat.</p>
            <div class="shot"><img src="/v7-daftar-obrolan-cak.app.png" alt="Daftar obrolan Cak.app"></div>
          </div>
          <div class="fc">
            <h3>Thread</h3>
            <p>Satu pesan, satu ruang diskusi. Obrolan utama tetap rapi.</p>
            <div class="shot"><img src="/v7-layar-thread-cak.app.png" alt="Layar thread Cak.app"></div>
          </div>
          <div class="fc">
            <h3>Tugas</h3>
            <p>Pesan arahan, jadi tugas. Penanggung jawab, tenggat, status.</p>
            <div class="shot"><img src="/v7-daftar-tugas-cak.app.png" alt="Daftar tugas Cak.app"></div>
          </div>
        </div>
      </div>
    </section>

    <!-- Tugas -->
    <section class="st" id="tugas">
      <div class="w">
        <h2>Dari obrolan sampai tugas selesai.</h2>
        <div class="pair">
          <figure><div class="ph"><img src="/v7-daftar-obrolan-cak.app.png" alt="Daftar obrolan Cak.app"></div><figcaption>Obrolan</figcaption></figure>
          <figure style="margin-top:48px"><div class="ph"><img src="/v7-daftar-tugas-cak.app.png" alt="Daftar tugas Cak.app"></div><figcaption>Tugas</figcaption></figure>
        </div>
      </div>
    </section>

    <!-- Perangkat -->
    <section class="st" id="perangkat">
      <div class="w">
        <h2>Perangkat</h2>
        <p class="sub" style="margin:12px auto 0;max-width:640px">Satu aplikasi, semua perangkat. Desktop, tablet, dan ponsel.</p>
        <div class="device-grid">
          <div class="dev">
            <div class="dev-frame desktop"><img src="/v7-daftar-obrolan-cak.app.png" alt="Daftar obrolan Cak.app"></div>
            <p>Desktop</p>
          </div>
          <div class="dev">
            <div class="dev-frame tablet"><img src="/v7-ruang-obrolan-dengan-tombol-3-balasan.png" alt="Ruang obrolan dengan tombol 3 balasan"></div>
            <p>Tablet</p>
          </div>
          <div class="dev">
            <div class="dev-frame phone"><img src="/v7-layar-thread-cak.app.png" alt="Layar thread Cak.app"></div>
            <p>Ponsel</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Paket -->
    <section class="st" id="paket">
      <div class="w">
        <h2>Paket</h2>
        <p class="sub" style="margin:12px auto 0;max-width:640px">Mulai gratis. Naik paket saat tim butuh.</p>
        <div class="pricing">
          <div class="pc">
            <h3>Free</h3>
            <div class="price">Rp0<small>/bln</small></div>
            <ul>
              <li>Chat pribadi & grup</li>
              <li>Hingga 5 anggota tim</li>
              <li>Tugas dasar</li>
            </ul>
            <a class="btn" href="#gabung">Coba Gratis</a>
          </div>
          <div class="pc featured">
            <h3>Plus</h3>
            <div class="price">Rp29.000<small>/bln</small></div>
            <ul>
              <li>Semua fitur Free</li>
              <li>Hingga 10 anggota tim</li>
              <li>Penyimpanan lebih besar</li>
              <li>Riwayat pesan lebih panjang</li>
            </ul>
            <a class="btn" href="#gabung">Pilih Plus</a>
          </div>
          <div class="pc">
            <h3>Pro</h3>
            <div class="price">Rp59.000<small>/bln</small></div>
            <ul>
              <li>Semua fitur Plus</li>
              <li>Anggota tak terbatas</li>
              <li>Analitik tim</li>
              <li>Dukungan 24/7</li>
            </ul>
            <a class="btn dk" href="#gabung">Pilih Pro</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Bantuan -->
    <section class="st" id="bantuan">
      <div class="w">
        <h2>Bantuan</h2>
        <p class="sub" style="margin:12px auto 0;max-width:640px">Temukan jawaban dan hubungi kami.</p>
        <div class="faq">
          <div class="fq">
            <h3>Bagaimana cara membuat tugas dari chat?</h3>
            <p>Ketuk tombol "+ Jadikan tugas" pada pesan di ruang obrolan. Tugas akan muncul di daftar tugas.</p>
          </div>
          <div class="fq">
            <h3>Apa itu Thread?</h3>
            <p>Thread adalah ruang diskusi terfokus pada satu pesan. Obrolan utama tetap rapi.</p>
          </div>
          <div class="fq">
            <h3>Bagaimana mengundang anggota tim?</h3>
            <p>Buka Pengaturan Tim, pilih Undang Anggota, lalu kirim tautan atau email undangan.</p>
          </div>
          <div class="fq">
            <h3>Apakah ada paket gratis?</h3>
            <p>Ya, paket Free tersedia untuk perorangan tanpa biaya.</p>
          </div>
        </div>
        <div style="margin-top:40px;text-align:center">
          <a class="btn" href="#">Hubungi Kami</a>
        </div>
      </div>
    </section>

    <!-- CTA -->
    <section class="cta" id="gabung">
      <img src="/v7-logo-cak.app.png" alt="Logo Cak.app"><h2>Coba Cak.app sekarang.</h2><a class="btn dk" href="#">Coba Gratis</a>
    </section>
  </main>

  <footer>
    <div class="w fr">
      <b style="color:#162136">Cak.app</b>
      <span class="sp"></span>
      <a href="#fitur">Fitur</a>
      <a href="#perangkat">Perangkat</a>
      <a href="#paket">Paket</a>
      <a href="#bantuan">Pusat bantuan</a>
      <a href="#">Kebijakan privasi</a>
      <a href="#">Syarat layanan</a>
      <span>© 2026 Sampulkreativ</span>
    </div>
  </footer>
</template>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const EN = {"Fitur":"Features","Perangkat":"Devices","Paket":"Plans","Bantuan":"Help","Pilih bahasa": "Select language", "Masuk": "Log in", "Coba Gratis": "Try for free", "Chat · Thread · Tugas": "Chat · Threads · Tasks", "Chat lebih terarah,": "Clearer chats,", "kerja lebih mudah": "easier work", "Satu aplikasi untuk ngobrol dan mengatur pekerjaan tim.": "One app to chat and organize your team’s work.", "Lihat Thread": "See Threads", "+ Jadikan tugas": "+ Make it a task", "3 balasan": "3 replies", "Tugas": "Tasks", "Obrolan": "Chats", "Satu pesan, satu ruang diskusi.": "One message, one discussion space.", "Obrolan utama tetap rapi.": "The main chat stays tidy.", "Ketuk 3 balasan": "Tap 3 replies", "Diskusi di sini": "Discuss here", "Dari obrolan sampai tugas selesai.": "From chat to done.", "Coba Cak.app sekarang.": "Try Cak.app now.", "Pusat bantuan": "Help center", "Kebijakan privasi": "Privacy policy", "Syarat layanan": "Terms of service", "Hubungi Kami": "Contact Us", "Paket": "Plans", "Perangkat": "Devices"}
  const ALT = {"Logo Cak.app": "Cak.app logo", "Pilih bahasa": "Select language", "Daftar obrolan Cak.app": "Cak.app chat list", "Ruang obrolan dengan tombol 3 balasan": "Chat room with a 3 replies button", "Layar thread Cak.app": "Cak.app thread screen", "Daftar tugas Cak.app": "Cak.app task list"}
  const b = document.getElementById('lgb')
  const m = document.getElementById('lgm')
  const lab = document.getElementById('lgl')
  function walk(l) {
    const w = document.createTreeWalker(document.body, NodeFilter.SHOW_TEXT)
    let n
    while (n = w.nextNode()) {
      if (n.parentNode && n.parentNode.closest && n.parentNode.closest('script,style')) continue
      if (n._o === undefined) n._o = n.nodeValue
      const k = (n._o || '').trim()
      if (!k) continue
      const t = (l === 'en' && EN[k]) ? EN[k] : k
      n.nodeValue = (n._o || '').replace(k, t)
    }
    document.querySelectorAll('[alt],[aria-label]').forEach(function (e) {
      ;['alt', 'aria-label'].forEach(function (a) {
        if (!e.hasAttribute(a)) return
        if (e['_' + a] === undefined) e['_' + a] = e.getAttribute(a)
        const o = e['_' + a]
        e.setAttribute(a, (l === 'en' && ALT[o]) ? ALT[o] : o)
      })
    })
  }
  function setLang(l, save) {
    document.documentElement.lang = l
    if (lab) lab.textContent = l.toUpperCase()
    if (m) m.querySelectorAll('button').forEach(function (x) { x.setAttribute('aria-selected', x.dataset.l === l ? 'true' : 'false') })
    walk(l)
    if (save) { try { localStorage.setItem('cak-lang', l) } catch (e) {} }
  }
  function toggle(o) { if (m) m.classList.toggle('on', o); if (b) b.setAttribute('aria-expanded', o ? 'true' : 'false') }
  if (b) b.addEventListener('click', function (e) { e.stopPropagation(); toggle(!m.classList.contains('on')) })
  if (m) m.addEventListener('click', function (e) { const x = e.target.closest('button[data-l]'); if (x) { setLang(x.dataset.l, true); toggle(false); b.focus() } })
  document.addEventListener('click', function () { toggle(false) })
  document.addEventListener('keydown', function (e) { if (e.key === 'Escape') { toggle(false); b.focus() } })
  let st = null
  try { st = localStorage.getItem('cak-lang') } catch (e) {}
  if (st === 'en') setLang('en', false)
})
</script>