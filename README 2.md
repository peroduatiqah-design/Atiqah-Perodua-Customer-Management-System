# Atiqah Perodua CRM — MVP 0.1

## Kandungan
- `index.html`: aplikasi CRM
- `manifest.webmanifest`: tetapan PWA
- `sw.js`: service worker untuk cache/offline shell
- `icon-192.png`, `icon-512.png`: ikon aplikasi

## Fungsi
Tambah/edit/padam customer, model/variant, bank, tarikh submit, status loan, follow-up, booking/VSO/delivery, carian, dashboard ringkas dan export CSV.

## Penting — jangan guna untuk data pelanggan sebenar dahulu
Ini ialah prototaip setempat. Rekod disimpan dalam `localStorage` pada browser/peranti semasa sahaja. Tiada penyegerakan cloud, backup automatik atau kawalan akses pelayan. PIN demo hanya menyembunyikan paparan; ia bukan encryption dan tidak melindungi data daripada orang yang boleh mengakses storan browser/peranti. Jangan masukkan nombor IC penuh, salinan IC, slip gaji, penyata bank atau dokumen sensitif.

Sebelum penggunaan sebenar, perlu tambah backend/database yang mempunyai authentication sebenar, encryption in transit/at rest, backup, audit log, kawalan akses, dan proses pemadaman/retention yang sesuai.

## Cara uji di komputer
Buka `index.html` dalam browser moden. Untuk PWA/offline dan pemasangan, host folder ini melalui HTTPS (contohnya hosting static yang menyokong HTTPS). `file://` sahaja tidak mencukupi untuk pemasangan PWA.

## Pasang di iPhone selepas di-host
1. Buka URL HTTPS aplikasi dalam Safari.
2. Tekan Share.
3. Pilih Add to Home Screen.
4. Tekan Add.

PIN demo pertama kali: tetapkan 4–6 digit apabila skrin meminta. Jika terlupa PIN, clear site data akan memadam PIN dan rekod setempat; export CSV dahulu jika perlu.
