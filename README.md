# SIMULASI BANSOS (Demo — Bukan Situs Resmi)

## Peringatan
Proyek ini adalah **simulasi interaktif** untuk demonstrasi alur pengecekan bantuan
sosial dan verifikasi OTP. Halaman ini **BUKAN** situs resmi pemerintah mana pun,
**tidak** meniru identitas instansi, dan **tidak** mengumpulkan data pribadi nyata.
Seluruh data masukan bersifat fiktif.

## Cara Mencatatkan
1. `npm install`
2. Salin `.env.example` ke `.env.local`, lalu isi (opsional):
   - `TELEGRAM_BOT_TOKEN` — token bot (buat via @BotFather)
   - `TELEGRAM_DEVELOPER_CHAT_ID` — chat ID akun Telegram **Anda sendiri**
   
   OTP hanya dikirim ke chat ID ini (whitelist pengembang), bukan ke nomor pengunjung.
3. `npm run dev` → buka `http://localhost:3000`

Tanpa variabel Telegram, kiriman OTP dinonaktifkan (logika tetap berjalan, kode
tersedia lewat `devCode` saat `NODE_ENV !== 'production'`).

## Script
- `npm run dev` — mode development (port 3000)
- `npm run build` — produksi build
- `npm run start` — jalankan hasil build
- `npm run lint` — lint

## Stack
Next.js 15 (App Router) · React 19 · TypeScript · Tailwind CSS v4 · lucide-react