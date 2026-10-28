# Uji Kamera WebRTC (demo)

Demo edukasi untuk mengirim kamera HP ke monitor browser laptop setelah izin kamera diberikan.

## Cara menerbitkan di GitHub Pages
1. Unggah `index.html`, `monitor.html`, dan `README.md` ke root repositori.
2. Di GitHub: **Settings → Pages**, pilih branch `main` dan folder `/ (root)`.
3. Tunggu deployment selesai. Buka URL Pages di HP untuk pengirim dan tambahkan `monitor.html` untuk laptop.

## Cara mencoba
1. Buat kode ruang acak minimal 8 karakter, misalnya rangkaian acak huruf/angka.
2. Buka halaman utama di HP, masukkan kode dan tekan **Hubungkan ruang**.
3. Tekan **Mulai kamera & kirim video**, lalu setujui izin kamera.
4. Di laptop, buka URL yang sama dengan akhiran `/monitor.html`, masukkan kode yang sama, tekan **Sambungkan monitor**.

## Catatan privasi dan teknis
- Kamera hanya aktif setelah tindakan pengguna dan persetujuan browser.
- Halaman ini tidak merekam atau menyimpan video.
- PeerJS Cloud digunakan sebagai signaling; koneksi lintas jaringan tidak dijamin dan beberapa jaringan memerlukan TURN relay khusus.
- Kode ruang bukan sistem autentikasi kuat. Jangan gunakan untuk hal sensitif atau membagikan kode ke pihak lain.
- Script PeerJS dimuat dari CDN pihak ketiga. Untuk penggunaan lebih serius, host dependensi sendiri dan gunakan signaling/TURN yang dikelola sendiri.
- Demo ini tidak mencatat kunjungan atau aktivitas tersembunyi.
