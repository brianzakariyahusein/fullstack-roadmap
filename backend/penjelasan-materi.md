# **🖥️ Bab 1: Dasar-dasar Komputer & Jaringan**

---

## **1.1 Cara Kerja Internet 🌍**

Internet adalah jaringan global yang menghubungkan miliaran perangkat di seluruh dunia. Internet memungkinkan kita untuk berkomunikasi antar komputer melalui protokol standar seperti **`TCP/IP`**, dan **`HTTP/HTTPS`**.

### **🔹 Bagaimana Data Dikirim di Internet?**

1. **Client mengirim permintaan (Request)** ke server melalui **Protokol HTTP/HTTPS**.
2. **Server menerima permintaan** dan memprosesnya.
3. **Server mengirimkan respon** kembali ke Client dalam bentuk **halaman web, data JSON, DLL.**
4. **Client menampilkan data** (Misalnya browser menampilkan website yang kita akses).

---

## **1.2 HTTP & HTTPS 📡**

### **🔹 Apa itu HTTP?**

HTTP **(HyperText Transfer Protocol)** adalah **Protokol Komunikasi** yang digunakan untuk bertukar informasi antara client (Browser) dan server.

Contoh permintaan HTTP:
**Request Body:**

```js
GET /home HTTP/1.1
Host: www.example.com
```

Server akan merespons dengan data yang diminta oleh client.

### **🔹 Perbedaan HTTP vs HTTPS**
| HTTP | HTTPS |
|------|------|
| Tidak dienkripsi | Data dienkripsi dengan SSL/TLS |
| Rentan terhadap serangan | Lebih aman dari peretas |
| Digunakan di website lama | Standar wajib untuk website modern |

🔹 **Kode Status HTTP**:
✅ **200 OK** → Permintaan berhasil.  
🚫 **404 Not Found** → Halaman tidak ditemukan.  
⚠️ **500 Internal Server Error** → Server mengalami masalah.  

---

## **1.3 DNS & Hosting 🌐**

🔹 **DNS (Domain Name System)** menerjemahkan **nama domain** menjadi **alamat IP**.  

🔹 **Jenis Hosting**:
1. **Shared Hosting** → Murah, digunakan bersama pengguna lain.
2. **VPS (Virtual Private Server)** → Lebih fleksibel, tapi butuh konfigurasi.
3. **Dedicated Hosting** → Mahal, tapi memiliki performa tinggi.
4. **Cloud Hosting** → Dapat diskalakan secara otomatis.

---

## **1.4 Dasar Networking & Sistem Operasi 🔗**

🔹 **IP Address**  
- **IPv4:** `192.168.1.1` (Terbatas, 4 miliar alamat unik).  
- **IPv6:** `2001:db8::ff00:42:8329` (Hampir tak terbatas).  

🔹 **TCP vs UDP**
| **TCP** (Transmission Control Protocol) | **UDP** (User Datagram Protocol) |
|--------------------------------|----------------------------|
| Stabil, memiliki error-checking | Lebih cepat, tanpa error-checking |
| Digunakan untuk Web, Email, FTP | Digunakan untuk Streaming, VoIP, Gaming |

🔹 **Keamanan Jaringan**
- **Firewall** → Melindungi sistem dengan memblokir lalu lintas berbahaya.
- **VPN (Virtual Private Network)** → Mengamankan komunikasi dengan enkripsi.

🔹 **Proses, Threads, dan Concurrency**
- **Proses (Process):** Program yang sedang berjalan di sistem operasi.
- **Threads:** Unit eksekusi dalam suatu proses, memungkinkan eksekusi multitasking.
- **Concurrency:** Kemampuan menjalankan beberapa tugas secara bersamaan untuk meningkatkan efisiensi sistem.

🔹 **Manajemen Sistem Operasi**
- **Manajemen Memori:** Mengalokasikan dan mengelola penggunaan RAM.
- **Manajemen I/O:** Mengatur komunikasi antara hardware dan software.
- **Interprocess Communication (IPC):** Cara komunikasi antara proses yang berjalan.

---

## **📝 Tugas Praktik**

✅ **Cek alamat IP-mu**:  
   - Buka **Command Prompt (Windows) / Terminal (Mac/Linux)** dan ketik:  
     ```
     ipconfig (Windows)
     ifconfig atau ip a (Linux/Mac)
     ```

✅ **Cek DNS website**:  
   - Buka terminal dan ketik:  
     ```
     nslookup google.com
     ```
   - Hasilnya menunjukkan IP dari server Google.

✅ **Melihat daftar proses yang berjalan di sistem**:  
   - **Windows**: Buka **Task Manager** (`Ctrl + Shift + Esc`) dan lihat tab **Processes**.
   - **Linux/Mac**: Buka terminal dan ketik:  
     ```
     ps aux
     top
     htop
     ```

---

## **🚀 Kesimpulan**

Memahami dasar komputer dan jaringan sangat penting sebelum mempelajari backend development. Dengan menguasai konsep-konsep ini, kamu akan lebih siap untuk membangun sistem yang aman dan scalable!

---
📩 **Ada pertanyaan? Jangan ragu untuk bertanya!** 😊

