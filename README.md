/* Genel Ayarlar */
body, html {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f4f4f4;
    scroll-behavior: smooth;
}

/* W3Schools Arka Plan Örneği: Sabit Görsel (Parallax Effect) */
#banner-sorunlar {
    background-image: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('img/banner-bg.jpg');
    height: 300px;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    text-align: center;
}

/* Menü ve Navigasyon */
header { background: #2c3e50; color: white; padding: 10px 0; }
.kutu { width: 80%; margin: auto; overflow: hidden; }
nav ul { padding: 0; list-style: none; display: flex; justify-content: flex-end; }
nav li { margin-left: 20px; }
nav a { color: white; text-decoration: none; font-weight: bold; }
.aktif { border-bottom: 3px solid #e74c3c; }

/* --- TİMELİNE (DÜZ ÇİZGİ) TASARIMI --- */
.timeline {
    position: relative;
    max-width: 1200px;
    margin: 50px auto;
}

/* Ortadaki Dikey Çizgi */
.timeline::after {
    content: '';
    position: absolute;
    width: 6px;
    background-color: #2c3e50;
    top: 0;
    bottom: 0;
    left: 50%;
    margin-left: -3px;
}

/* İçerik Kutuları */
.konteynir {
    padding: 10px 40px;
    position: relative;
    background-color: inherit;
    width: 50%;
    box-sizing: border-box;
}

/* Çizgi Üzerindeki Noktalar */
.konteynir::after {
    content: '';
    position: absolute;
    width: 25px;
    height: 25px;
    right: -17px;
    background-color: white;
    border: 4px solid #e74c3c;
    top: 15px;
    border-radius: 50%;
    z-index: 1;
}

.sol { left: 0; }
.sag { left: 50%; }

.sag::after { left: -17px; }

.icerik {
    padding: 20px 30px;
    background-color: white;
    position: relative;
    border-radius: 6px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

/* Mobil Uyumluluk (Ekran küçülünce çizgi sola kayar) */
@media screen and (max-width: 600px) {
    .timeline::after { left: 31px; }
    .konteynir { width: 100%; padding-left: 70px; padding-right: 25px; }
    .konteynir::after { left: 15px; }
    .sag { left: 0; }
}

footer { text-align: center; padding: 20px; background: #2c3e50; color: white; margin-top: 50px; }
