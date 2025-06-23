![Foto](https://files.catbox.moe/n1onoz.jpg)

### Penjelasan 
ini adalah script node.js berbasis express + axios yang digunakan untuk keperluan edukasi dan riset keamanan jaringan, khususnya dalam melakukan simulasi traffic request secara masif melalui endpoint API.

> hanya untuk pembelajaran, testing, dan audit sistem sendiri. dilarang keras disalahgunakan!

---

### Fitur
- di jalan kan via API: `GET /api/attack/:url`
- random user-agent, referer, encoding, dll.
- built-in header spoof
- multi request async otomatis
- tanpa tools tambahan

---

### Instalasi dan jalankan 

1. clone repo:
```bash
git clone https://github.com/HanX-ID/ddos-api
cd ddos-api
```
2. install module:
```
npm install
```
3. jalankan:
```
npm start
# atau
node index.js
```

---

### Cara melakukan request attack

akses lewat browser atau curl:
```
http://localhost:8080/api/attack/https://target.com
```
contoh:
```
curl "http://localhost:8080/api/attack/https://example.com"
```

---

### Custom Request 

ubah jumlah request, edit di index.js:
```javascript
if (i >= 2000) clearInterval(interval);
```
---

#### Disclaimer!

> script ini disediakan untuk pembelajaran, pengujian sistem sendiri, dan auditing. saya tidak bertanggung jawab atas penyalahgunaan pengguna.

****Author**** [HanX](https://github.com/HanX-ID)
