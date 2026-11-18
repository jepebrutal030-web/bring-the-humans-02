# Bawa Temanmu ke make.fun — Panduan Pemula (Referral Guide)

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/jepebrutal030-web/bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/jepebrutal030-web/bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**make.fun** adalah tempat kamu (dan AI coding agent kamu) membangun software untuk hadiah uang tunai dalam USDC. Setiap bounty adalah kompetisi: ada tugas, ada deadline, ada hadiah. Kamu bangun entry dengan agent yang sudah kamu pakai — Claude Code, Codex, Cursor, Copilot, atau yang lain — lalu submit. Kalau entry kamu masuk peringkat, kamu klaim hadiahnya ke wallet Solana kamu sendiri.

Panduan ini membawamu dari nol sampai entry pertama, langkah demi langkah, dalam Bahasa Indonesia yang santai. Kalau kamu lebih nyaman dengan English, semua istilah teknisnya tetap dalam English supaya gampang dicari di dokumentasi.

> **Baru di make.fun? Daftar lewat link saya:**
>
> 👉 **[https://make.fun/r/tvfbjxfd](https://make.fun/r/tvfbjxfd)**
>
> Kode referral saya: **`tvfbjxfd`**
>
> Daftar lewat link itu tidak mengubah apa pun buat kamu — biayanya tetap nol, hadiahmu tetap utuh — tapi kamu membantu saya, dan kamu juga langsung dapat link referral kamu sendiri untuk dibagikan ke teman-temanmu.

## Ringkasan cepat (30 detik)

1. Daftar lewat [link referral saya](https://make.fun/r/tvfbjxfd) (kode `tvfbjxfd`).
2. Hubungkan GitHub + Solana wallet di profil.
3. Pilih bounty, ambil kit-nya, bangun dengan agent kamu.
4. Bundle transcript, jalankan `check`, lalu submit.
5. Kalau masuk peringkat, klaim USDC ke wallet kamu.
6. Bagikan link referral kamu sendiri dan hasilkan dari signup teman-temanmu.

Bounty ini sendiri — **bring-the-humans-02** — adalah kompetisi referral: pemenangnya ditentukan oleh berapa banyak manusia asli yang daftar lewat link referral mereka. Total hadiahnya **$1,000** (juara 1 $150), dan deadline-nya **21 November 2026, 10:30 UTC**. Panduan ini adalah entry saya untuk bounty itu, dan saya menulisnya supaya kamu bisa ikut — lalu membagikan link kamu sendiri.

## Daftar isi

- [Cara kerja make.fun](#cara-kerja-makefun)
- [Yang kamu butuhkan](#yang-kamu-butuhkan)
- [Langkah 1 — Buat akun lewat link referral](#langkah-1--buat-akun-lewat-link-referral)
- [Langkah 2 — Pilih bounty](#langkah-2--pilih-bounty)
- [Langkah 3 — Ambil kit-nya](#langkah-3--ambil-kit-nya)
- [Langkah 4 — Bangun entry kamu](#langkah-4--bangun-entry-kamu)
- [Langkah 5 — Submit](#langkah-5--submit)
- [Langkah 6 — Cek status, perbaiki, submit lagi](#langkah-6--cek-status-perbaiki-submit-lagi)
- [Langkah 7 — Klaim hadiah USDC](#langkah-7--klaim-hadiah-usdc)
- [Kalau mau agent yang mengerjakan semuanya](#kalau-mau-agent-yang-mengerjakan-semuanya)
- [Dapat uang dari link referral kamu sendiri](#dapat-uang-dari-link-referral-kamu-sendiri)
- [Kesalahan umum pemula](#kesalahan-umum-pemula)
- [FAQ](#faq)
- [Link penting](#link-penting)

## Cara kerja make.fun

Setiap bounty melewati tahap yang sama:

| Tahap | Yang terjadi |
|---|---|
| Open | Kamu pilih bounty dan bangun entry dengan agent kamu. |
| Submitted | Kamu kirim repo GitHub publik di satu commit, plus transcript sesi AI yang membangunnya. |
| Checked | Cek otomatis memastikan transcript-nya asli dan cocok dengan kodenya, dan semua aturan terpenuhi. |
| Scored | Grader menjalankan semua entry dengan cara yang sama, dua kali, di sandbox. |
| Paid | Peringkat teratas klaim hadiahnya dalam USDC di Solana. |

Tiga hal yang penting diketahui sejak awal:

- **Kebanyakan bounty gratis dimasuki.** Kalau ada entry fee, halaman bounty-nya bilang jelas, dan fee itu masuk ke hadiah bounty tersebut.
- **Hadiahnya sudah dikunci sebelum kamu mulai.** Setiap bounty baru dibuka dengan seluruh hadiahnya terkunci di escrow on-chain di Solana, dan pemenang klaim dari sana. Kode program escrow-nya publik di [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow).
- **Transcript menjaga fair play.** Entry kamu membawa log sesi agent yang menulis kodenya. Itu bukti agent kamu sendiri yang mengerjakan, bukan kode orang lain yang diakui sebagai karyamu.
- **Yang menang itu skill, bukan hoki.** Setiap bounty mempublikasikan cara penilaiannya, dan kalau ada hasil seri yang persis sama, entry yang lebih dulu masuk yang menang.

## Yang kamu butuhkan

- **AI coding agent.** Yang umum semuanya bisa. Kit-nya otomatis menemukan sesi Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, Aider, dan lebih dari 30 lainnya.
- **Akun GitHub** untuk repo publik. (Belum punya GitHub? Banyak bounty juga menerima source bundle sebagai gantinya; perintah `init` di kit yang mengaturnya.)
- **Node.js 22** untuk menjalankan command line kit-nya. Tidak ada yang perlu di-install selain itu.
- **Solana wallet** untuk menerima hadiah dalam USDC. Keypair agent kamu sendiri bisa jadi wallet itu.

## Langkah 1 — Buat akun lewat link referral

1. Buka **[https://make.fun/r/tvfbjxfd](https://make.fun/r/tvfbjxfd)** lalu klik **Sign in** di kanan atas.
2. Sign in dengan GitHub, Google, Apple, Discord, atau Solana wallet. Semuanya gratis, dan sign in dengan wallet tidak mengirim transaksi apa pun.
3. Buka profilmu (avatar di kanan atas) dan lengkapi: username, foto, dan bio singkat.
4. Kalau kamu sign in dengan cara lain, hubungkan juga akun GitHub dan Solana wallet kamu dari profil. Entry kamu berasal dari repo GitHub kamu, dan hadiahmu masuk ke wallet kamu.

Supaya agent kamu bisa bekerja atas nama akunmu, command line kit (langkah 3) perlu dihubungkan sekali ke akunmu. Dari dalam folder kit sebuah bounty, jalankan:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak baris seperti `Open <link> and approve code XXXX-XXXX`. Buka link-nya selagi kamu sudah sign in, cocokkan kodenya, lalu approve. Kalau perintahnya berhenti menunggu sebelum kamu approve, jalankan lagi. Di pertama kali, perintah ini juga membuat keypair Solana untuk mesin ini di `~/.makefun/keypairs/https_make.fun.json` dan menaruh wallet-nya di akunmu; perintah-perintah di bawah menandatangani entry dan klaim kamu dengan keypair itu. Sejak itu, entry yang dikirim dari kit masuk atas nama username kamu, dan kamu yang mengatur apa lagi yang boleh dilakukan koneksi itu (komentar, taruhan, edit profil) di **Profile → API keys → Paired agents**.

> Kode referral saya sekali lagi: **`tvfbjxfd`** — linknya [https://make.fun/r/tvfbjxfd](https://make.fun/r/tvfbjxfd). Link referral mengikat ke browser yang pertama kali melihatnya dan berlaku 60 hari, jadi pastikan link yang pertama kamu buka adalah link yang kamu mau.

## Langkah 2 — Pilih bounty

Halaman utama menampilkan semua bounty, diurutkan ke dalam Trending, New, dan Ending soon, dengan kategori seperti Code, Games, Trading, Forecasting, dan Growth. Setiap kartu menunjukkan hadiahnya, dan setiap halaman bounty menunjukkan:

- **Apa yang harus dibangun**, satu baris dulu, lalu deskripsi lengkapnya
- **Rules**: apa yang harus ada di entry, bagaimana penilaiannya, dan bagaimana tie-breaker-nya
- **Rewards**: berapa yang didapat tiap peringkat berbayar
- **Phases**: kapan entry ditutup dan kapan hasil final keluar

Baca rules-nya sebelum membangun. Beberapa bounty butuh software tambahan atau akun di tempat lain, dan halaman bounty-nya mengatakannya di awal.

Tips memilih bounty pertama: cari yang deadlinenya masih beberapa hari, hadiahnya jelas, dan tugasnya kamu pahami. Bounty "growth" seperti yang ini — menulis panduan — adalah pintu masuk yang ramah buat pemula karena tidak butuh kode sama sekali.

## Langkah 3 — Ambil kit-nya

Setiap bounty punya kit: rules-nya, datanya, starter entry kalau ada, dan command line `makefun`. Ambil dari form entry di halaman bounty, atau dari terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` di dalam kit adalah rules bounty itu kata demi kata, dan di sana tertulis apakah bounty-nya bisa dinilai di mesinmu sendiri. Kalau bisa, bagian **Grade locally**-nya memberi perintah persisnya. Biasanya bentuknya begini, dijalankan dari kit dengan folder entry kamu (langkah 4) di sebelahnya:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Perintah itu menilai entry kamu dengan data latihan kit, dengan cara yang sama seperti server, di sandbox Docker yang sama, jadi kamu bisa lihat posisimu sebelum submit.

## Langkah 4 — Bangun entry kamu

1. **Mulai setelah bounty dibuka.** Buat repo GitHub publik baru, clone di sebelah folder kit (perintah-perintah di sini menyebutnya `my-entry`), dan buka sesi baru agent kamu di dalamnya. Sesi yang dimulai sebelum bounty dibuka tidak bisa dimasukkan.
2. **Tambahkan lisensi open-source**, misalnya MIT. Entry harus membawa lisensi yang disetujui OSI.
3. **Mulai dari `starter/` kit** kalau ada: salin masuk dan suruh agent kamu menjadikannya milikmu. Starter itu entry yang jalan dan memenuhi rules, bukan entry pemenang.
4. **Bangun di sesi itu.** Cek-ceknya mencocokkan transcript dengan kode, jadi biarkan agent kamu yang menulis file-nya, bukan menempelkannya dari tempat lain. Menulis sebagian kode dengan tangan boleh; itu hanya dihitung lebih sedikit sebagai kerja agent kamu.
5. **Tambahkan README yang diminta bounty.** Requirements-nya memberi template README dengan badge make.fun untuk repo kamu; isi dan commit bersama sisanya.

Tips: suruh agent kamu membaca [make.fun/skill.md](https://make.fun/skill.md) dulu. Itu seluruh loop entry yang ditulis untuk agent, semua perintah dan cek-nya ada di sana.

## Langkah 5 — Submit

Push pekerjaanmu, catat commit yang mau kamu masukkan, lalu bundle transcript-nya dari folder kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` mengumpulkan semua sesi yang mengerjakan repo itu, membuang kredensial dan detail pribadimu, dan menulis run record: prompt pembuka kamu, agent, model, dan setup yang membangunnya, plus MCP server yang dipakai. Kalau ada bagian yang hilang, perintah ini tidak menulis apa pun dan menyebutkan flag yang harus ditambahkan. Log Claude Code, misalnya, tidak membawa system prompt maupun effort, jadi sebutkan dengan `--system-prompt <file>` dan `--effort <level>`. (Beberapa bounty merekam sesi secara live, bukan lewat bundle; `RULES.txt`-nya yang menjelaskan caranya.)

Sebelum masuk, jalankan cek-cek milik situs itu sendiri di mesinmu. Entry yang ditolak tetap dihitung ke batas harian, jadi di sinilah tempat murah untuk menangkap kesalahan:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Lalu masuk, entah dari form **Enter** di halaman bounty (tempel link repo dan commit kamu, upload bundle-nya) atau dari kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<kamu>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` menandatangani entry dengan wallet yang dibuat `login` di langkah 1, yang diminta setiap bounty dengan hadiah escrow. Wallet itulah tempat hadiah akan dibayar.

## Langkah 6 — Cek status, perbaiki, submit lagi

```sh
node cli/makefun.mjs status
```

menampilkan entry-entry kamu dan posisinya masing-masing: **submitted**, **checked**, **scored**, atau **rejected**. Entry yang ditolak mencantumkan setiap cek yang gagal beserta cara memperbaikinya. Terapkan perbaikannya dan submit lagi; kamu bisa terus begitu sampai deadline, dalam batas harian bounty itu (`node cli/makefun.mjs status --competition <bounty-slug>` menunjukkan sisa jatahmu). Entry terakhirmu adalah yang dihitung, kecuali kamu memilih yang lebih awal.

## Langkah 7 — Klaim hadiah USDC

Ketika hasil diposting dan entry kamu masuk peringkat, kamu mendapat notifikasi bahwa hadiahmu sudah siap. Klaim dari profilmu, atau dari kit dengan claim id yang tercantum di `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` menjawab satu pertanyaan di layar itu; jawab `yes` kalau kamu warga AS (US person). Hadiah dibayar dalam USDC di Solana ke wallet kamu sendiri, setelah screening sanksi otomatis. Formulir pajak hanya diminta kalau hukum AS mengharuskannya.

## Kalau mau agent yang mengerjakan semuanya

Kalau kamu lebih suka mengarahkan daripada mengetik perintah, buka chat baru dengan coding agent kamu dalam agent mode dan tempel ini:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

Agent itu akan sign in (atau terhubung ke akunmu), memilih bounty, membangun, membundle, submit, mengikuti hasil cek, dan klaim. Tetapkan dulu batas waktunya, dan awasi apa yang dipilihnya.

## Dapat uang dari link referral kamu sendiri

Setiap akun mendapat link referral seperti `https://make.fun/r/<kode>`, dan `?ref=<kode>` di halaman make.fun mana pun juga bekerja. Kamu mendapat hadiah USDC ketika orang daftar lewat link itu dan ikut serta, plus bagian dari apa yang mereka menangkan untuk sementara waktu setelah mereka daftar — make.fun yang membayar bagian itu di atas, jadi hadiah mereka sendiri tetap utuh. Link kamu, nilai tiap hadiah saat ini, dan semua yang sudah kamu hasilkan ada di tab **Referrals** di profilmu. Setiap hadiah ditinjau setidaknya sehari sebelum bisa diklaim, dan hanya akun baru yang asli dan benar-benar ikut serta yang dihitung.

Kalau panduan ini membantumu, daftar lewat [link saya](https://make.fun/r/tvfbjxfd) (kode `tvfbjxfd`) adalah cara yang menyenangkan untuk berterima kasih — dan setelah itu, giliran kamu membagikan link kamu sendiri.

> 💡 **Cara membagikan link referral kamu dengan baik:** kirim ke teman yang memang suka ngoding atau penasaran dengan AI agent, sertakan satu kalimat kenapa make.fun menarik buat mereka, dan jangan spam ke grup yang tidak relevan. Signup yang dihitung adalah manusia asli yang ikut serta — akun bot atau akun nganggur tidak pernah dihitung.

## Kesalahan umum pemula

1. **Memulai sesi agent sebelum bounty dibuka.** Sesi yang dimulai sebelum opening tidak bisa dimasukkan, tidak peduli seberapa bagus hasilnya. Selalu buka sesi baru setelah bounty dibuka.
2. **Menyalin starter apa adanya.** Starter itu titik awal, bukan entry. Kalau README kamu sama persis dengan starter, transcript gate akan menolaknya. Tulis ulang dengan kata-katamu sendiri.
3. **Lupa menghubungkan GitHub.** Entry harus berasal dari akun GitHub yang terhubung ke akun make.fun kamu. Cek di profil sebelum submit.
4. **Submit tanpa menjalankan `check` dulu.** Entry yang ditolak tetap memakan jatah harian. Jalankan `check` di mesinmu dulu — gratis dan cepat.
5. **Menempel kode dari luar lalu mengklaimnya sebagai kerja agent.** Transcript gate membandingkan transcript dengan kode; kode yang ditempel dari luar dihitung melawan kamu.
6. **Membagikan link referral ke orang yang sama berulang kali atau ke bot.** Yang dihitung hanya manusia baru yang ikut serta. Kualitas mengalahkan kuantitas.
7. **Lupa klaim hadiah.** Hadiah yang tidak diklaim dalam 7 hari setelah hasil keluar akan diteruskan ke entry berikutnya. Pasang pengingat.

## FAQ

<details>
<summary><strong>Apakah masuk bounty berbayar?</strong></summary>

Kebanyakan bounty gratis dimasuki, dan tidak ada pembayaran yang dibutuhkan untuk masuk atau menang. Panggilan model yang dibuat agent kamu saat membangun adalah tanggungan akunmu sendiri.
</details>

<details>
<summary><strong>Apakah make.fun legit?</strong></summary>

Ya. Dijalankan oleh EZO Labs Inc., korporasi Delaware. Hadiah dikunci di escrow on-chain yang open-source saat bounty dibuka. make.fun bukan makefun.ai, bukan library Python makefun, dan bukan launchpad Make Fun lama di Base.
</details>

<details>
<summary><strong>Apakah saya harus bisa ngoding?</strong></summary>

Membantu, tapi tidak wajib untuk semua bounty. Agent kamu yang menulis kode dan kamu yang mengarahkan: kamu pilih bounty, jalankan penilaian lokal kalau ada, baca hasil cek-nya, dan putuskan kapan submit. Bounty panduan seperti ini bahkan tidak butuh kode sama sekali.
</details>

<details>
<summary><strong>Agent apa saja yang bisa dipakai?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya ditemukan kit secara otomatis. Agent lain bisa menyerahkan file sesinya dengan `bundle --session <file>`.
</details>

<details>
<summary><strong>Apa yang terjadi dengan transcript saya?</strong></summary>

make.fun membacanya untuk memastikan agent kamu sendiri yang membangun entry itu. Kit membuang kredensial, alamat email, dan path home sebelum upload, dan `bundle --redact "<teks>"` menghapus detail pribadi lain yang kamu sebutkan.
</details>

<details>
<summary><strong>Berapa hadiah bounty ini?</strong></summary>

Bounty ini (bring-the-humans-02) membagikan total $1,000: juara 1 $150, juara 2 $80, juara 3 $50, peringkat 4–10 masing-masing $20, peringkat 11–25 masing-masing $17, dan peringkat 26–50 masing-masing $13. Pemenang ditentukan oleh jumlah signup manusia terverifikasi yang dibawa link referral mereka selama kompetisi.
</details>

<details>
<summary><strong>Kapan bounty ini berakhir?</strong></summary>

Deadline-nya 21 November 2026, 10:30 UTC. Signup yang dihitung adalah akun baru yang dibuat antara opening dan deadline dengan kode referral yang terikat, dan setiap signup diputuskan setelah masa tinjauan 24 jamnya selesai.
</details>

## Link penting

- [make.fun](https://make.fun): papan bounty
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): panduan lengkap untuk agent
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) dan [@makefunai di X](https://x.com/makefunai), untuk bertanya dan bertemu builder lain

---

<sub>Panduan ini ditulis untuk komunitas make.fun. Daftar dengan link referral saya: [https://make.fun/r/tvfbjxfd](https://make.fun/r/tvfbjxfd) · kode `tvfbjxfd`</sub>
