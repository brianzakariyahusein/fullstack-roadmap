# **🔥 Bab 2: Pemrograman Backend (JavaScript - Node.js)**  

## **2.1 Dasar-dasar JavaScript**  
JavaScript adalah bahasa pemrograman yang awalnya dibuat untuk pengembangan frontend, tetapi kini juga banyak digunakan di backend melalui **Node.js**.  

### **🔹 Variabel & Tipe Data**  
Di JavaScript, kita bisa mendeklarasikan variabel dengan tiga cara:  
```js
var nama = "Brian"; // Bisa diubah, tidak direkomendasikan
let umur = 18; // Bisa diubah, lebih fleksibel
const negara = "Indonesia"; // Tidak bisa diubah
```

**Tipe Data di JavaScript:**  
- **String** → `"Hello"`
- **Number** → `123`
- **Boolean** → `true` atau `false`
- **Array** → `[1, 2, 3]`
- **Object** → `{ nama: "Brian", umur: 18 }`
- **Null & Undefined** → `null`, `undefined`

---

### **🔹 Operator di JavaScript**  
JavaScript memiliki berbagai operator untuk melakukan operasi matematika dan logika:
```js
let a = 10;
let b = 5;
console.log(a + b); // 15 (Penjumlahan)
console.log(a - b); // 5 (Pengurangan)
console.log(a * b); // 50 (Perkalian)
console.log(a / b); // 2 (Pembagian)
console.log(a % b); // 0 (Modulus)
```

---


















































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































### **🔹 Struktur Kontrol (Kondisional & Perulangan)**  
#### **1. If-Else**  
```js
let nilai = 80;
if (nilai >= 75) {
    console.log("Lulus");
} else {
    console.log("Tidak Lulus");
}
```

#### **2. Switch-Case**  
```js
let hari = "Senin";
switch (hari) {
    case "Senin":
        console.log("Hari kerja");
        break;
    case "Minggu":
        console.log("Hari libur");
        break;
    default:
        console.log("Hari tidak diketahui");
}
```

#### **3. Perulangan (Looping)**  
```js
for (let i = 0; i < 5; i++) {
    console.log("Iterasi ke-", i);
}
```

```js
let j = 0;
while (j < 5) {
    console.log("Loop ke-", j);
    j++;
}
```

---

## **2.2 Asynchronous JavaScript**  
JavaScript berjalan secara **single-threaded**, sehingga eksekusi kode dilakukan satu per satu. Namun, dengan **asynchronous programming**, kita bisa menjalankan beberapa tugas tanpa menunggu yang lain selesai.  

### **🔹 Callback**  
```js
function prosesData(callback) {
    setTimeout(() => {
        console.log("Data diproses");
        callback();
    }, 2000);
}

prosesData(() => {
    console.log("Selesai");
});
```

### **🔹 Promise**  
```js
let janji = new Promise((resolve, reject) => {
    let sukses = true;
    if (sukses) {
        resolve("Berhasil");
    } else {
        reject("Gagal");
    }
});

janji.then(res => console.log(res)).catch(err => console.log(err));
```

### **🔹 Async/Await**  
```js
async function getData() {
    let hasil = await janji;
    console.log(hasil);
}
getData();
```

---

## **2.3 Node.js & Package Management**  
Node.js memungkinkan JavaScript berjalan di server, bukan hanya di browser.

### **🔹 Instalasi Node.js & npm**  
1. **Download Node.js** di [nodejs.org](https://nodejs.org/).
2. **Cek versi Node.js**:  
   ```sh
   node -v
   ```
3. **Cek versi npm (Node Package Manager)**:  
   ```sh
   npm -v
   ```

### **🔹 Membuat Project Node.js**  
```sh
mkdir project-backend
cd project-backend
npm init -y
```

### **🔹 Menggunakan Package npm**  
```sh
npm install express
```

```js
const express = require("express");
const app = express();

app.get("/", (req, res) => {
    res.send("Hello, Backend!");
});

app.listen(3000, () => console.log("Server berjalan di port 3000"));
```

---

## **📝 Tugas Praktik**  
✅ **Buat program JavaScript sederhana** menggunakan perulangan dan kondisi.  
✅ **Gunakan Promise atau Async/Await** untuk memahami asynchronous programming.  
✅ **Instal dan jalankan server Node.js** menggunakan Express.js.  

---

## **🚀 Kesimpulan**  
Memahami JavaScript dasar dan Node.js adalah langkah awal yang penting sebelum mendalami backend development lebih lanjut. Pastikan kamu sudah nyaman dengan konsep-konsep ini sebelum lanjut ke API Development!

---
📩 **Ada pertanyaan? Jangan ragu untuk bertanya!** 😊

