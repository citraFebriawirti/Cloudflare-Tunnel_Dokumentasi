# 🚀 Step-by-Step Deploy Laravel via Cloudflare Tunnel (Gratis)
## 💡 Keunggulan:

- ✅ **Tanpa batas bandwidth**
- ✅ **Stabil**
- ✅ **Gratis**

---

## 🛠️ 1. Install `cloudflared`

### Untuk Windows:
Unduh dari tautan resmi Cloudflare:  
🔗 [Install cloudflared - Cloudflare Docs](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/install-and-setup/installation)

## 2. Letakkan di Folder Proyek Laravel atau Tambahkan ke PATH

Misalnya kamu punya `cloudflared.exe` di:  
### ✅ Cara Tambahkan `cloudflared.exe` ke PATH di Windows:

1. **Pindahkan `cloudflared.exe` ke folder tetap**, misalnya:

2. **Salin path folder-nya:**
- Buka File Explorer
- Klik di kolom alamat
- Salin:
  ```
  C:\cloudflare-tunnel
  ```
  ![image](https://github.com/user-attachments/assets/d09d24fc-a0ec-423e-9b35-dece363045be)


3. **Buka Pengaturan Environment Variables:**
- Klik Start → Cari: `Environment Variables`
- Pilih: **Edit the system environment variables**
- Klik tombol: **Environment Variables...**

4. **Tambahkan ke PATH:**
- Di bagian **User variables** atau **System variables**:
  - Klik pada `Path` → klik **Edit...**
  - Klik **New** → tempelkan:
    ```
    C:\cloudflare-tunnel
    ```
- Klik **OK** di semua jendela hingga tertutup

  ![image](https://github.com/user-attachments/assets/51a4b6db-6bb1-43f4-8b25-491c3c8df15d)


5. **Restart** Command Prompt atau PowerShell

6. **Coba tes perintah:**
```bash
cloudflared --version
```
![image](https://github.com/user-attachments/assets/fd96cfb9-47e2-45b9-a6c8-4ccbdbfaf7f6)


## 3. Jalankan Cloudflare Tunnel
#### Setelah cloudflared ditambahkan ke PATH, jalankan:
```bash
cloudflared tunnel --url http://localhost:8000
```
![image](https://github.com/user-attachments/assets/c5336ff6-4f2b-4459-a45f-1f4f3f98a569)

## 4. Akses URL Publik
#### Jika berhasil, akan muncul URL acak seperti:
```bash
https://your-project-name.trycloudflare.com
```
![image](https://github.com/user-attachments/assets/ddf6bcc0-0410-4353-aae4-3d120c8ad114)

✅ URL ini bisa diakses publik.
 

