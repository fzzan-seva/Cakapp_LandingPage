<template>
  <div style="background:#fff;position:sticky;top:0;z-index:10">
    <div style="max-width:1200px;margin:0 auto;padding:0 32px;box-sizing:border-box;height:76px;display:flex;align-items:center;gap:32px">
      <div style="display:flex;align-items:center;gap:12px">
        <img src="/v7-logo-cak.app.png" alt="Logo Cak.app" style="width:40px;height:40px;display:block">
        <b style="font-size:22px;color:#162136">Cak.app</b>
      </div>
      <div style="flex:1"></div>
      <a class="nv" href="#/fitur" style="color:#162136;font-size:16px">Fitur</a>
      <a class="nv" href="#/perangkat" style="color:#162136;font-size:16px">Perangkat</a>
      <a class="nv" href="#/paket" style="color:#162136;font-size:16px">Paket</a>
      <a class="nv" href="#/bantuan" style="color:#162136;font-size:16px">Bantuan</a>
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
      <button @click="go('/')" style="background:#a5bf98;color:#162136;border:0;border-radius:40px;padding:12px 24px;font-size:16px;font-weight:600;font-family:inherit;line-height:1.2">Coba Gratis</button>
    </div>
  </div>

  <nav class="mobile-nav">
    <a href="#/fitur">Fitur</a>
    <a href="#/perangkat">Perangkat</a>
    <a href="#/paket">Paket</a>
    <a href="#/bantuan">Bantuan</a>
  </nav>

  <component :is="currentView" />

  <footer>
    <div class="w fr">
      <b style="color:#162136">Cak.app</b>
      <span class="sp"></span>
      <a href="#/fitur">Fitur</a>
      <a href="#/perangkat">Perangkat</a>
      <a href="#/paket">Paket</a>
      <a href="#/bantuan">Bantuan</a>
      <a href="#">Kebijakan privasi</a>
      <a href="#">Syarat layanan</a>
      <span>© 2026 Sampulkreativ</span>
    </div>
  </footer>
</template>

<script setup>
import { ref, computed, onMounted } from 'vue'
import Home from './pages/Home.vue'
import Fitur from './pages/Fitur.vue'
import Perangkat from './pages/Perangkat.vue'
import Paket from './pages/Paket.vue'
import Bantuan from './pages/Bantuan.vue'

const route = ref(window.location.hash.replace(/^#/, '') || '/')
if (!route.value.startsWith('/')) route.value = '/' + route.value

function parseRoute(h) {
  const r = (h || window.location.hash).replace(/^#/, '') || '/'
  return r.startsWith('/') ? r : '/' + r
}

function go(path) {
  route.value = path
  window.location.hash = '#' + path
  window.scrollTo(0, 0)
}

window.addEventListener('hashchange', () => { route.value = parseRoute() })

const currentView = computed(() => {
  if (route.value === '/fitur') return Fitur
  if (route.value === '/perangkat') return Perangkat
  if (route.value === '/paket') return Paket
  if (route.value === '/bantuan') return Bantuan
  return Home
})

onMounted(() => {
  const EN = {"Fitur":"Features","Perangkat":"Devices","Paket":"Plans","Bantuan":"Help","Pilih bahasa": "Select language", "Masuk": "Log in", "Coba Gratis": "Try for free", "Chat · Thread · Tugas": "Chat · Threads · Tasks", "Chat lebih terarah,": "Clearer chats,", "kerja lebih mudah": "easier work", "Satu aplikasi untuk ngobrol dan mengatur pekerjaan tim.": "One app to chat and organize your team’s work.", "Lihat Thread": "See Threads", "+ Jadikan tugas": "+ Make it a task", "3 balasan": "3 replies", "Tugas": "Tasks", "Obrolan": "Chats", "Satu pesan, satu ruang diskusi.": "One message, one discussion space.", "Obrolan utama tetap rapi.": "The main chat stays tidy.", "Ketuk 3 balasan": "Tap 3 replies", "Diskusi di sini": "Discuss here", "Dari obrolan sampai tugas selesai.": "From chat to done.", "Coba Cak.app sekarang.": "Try Cak.app now.", "Pusat bantuan": "Help center", "Kebijakan privasi": "Privacy policy", "Syarat layanan": "Terms of service", "Paket": "Plans", "Pusat Bantuan": "Help Center", "Mulai gratis. Naik paket saat tim butuh.": "Start free. Upgrade when your team needs more.", "Free": "Free", "Plus": "Plus", "Pro": "Pro", "Hubungi Kami": "Contact Us"}
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