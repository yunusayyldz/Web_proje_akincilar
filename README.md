# 🚫 SANAL BAHİS VE KUMAR BAĞIMLILIĞI İLE MÜCADELE PLATFORMU
### **"Farkında Ol, Özgür Kal" | Akıncılar Proje Grubu**

<div align="center">
  <img src="https://img.shields.io/badge/Hafta-SUNUM%20HAFTASI-red?style=for-the-badge&logo=prezi" alt="Sunum">
  <img src="https://img.shields.io/badge/Versiyon-V2.0%20(Visual%20Update)-blue?style=for-the-badge" alt="Versiyon">
  <img src="https://img.shields.io/badge/Grup-AKINCILAR-black?style=for-the-badge" alt="Grup">
  <br>
  <img src="https://img.shields.io/badge/Dil-HTML5-orange?style=flat-square&logo=html5">
  <img src="https://img.shields.io/badge/Stil-CSS3-blue?style=flat-square&logo=css3">
  <img src="https://img.shields.io/badge/Tasarım-Responsive-green?style=flat-square">
</div>

---

## 📝 PROJE VİZYONU
Bu proje, üniversite gençliği arasında sessiz bir pandemi gibi yayılan **sanal bahis ve kumar bağımlılığına** karşı dijital bir set çekmek amacıyla hazırlanmıştır. Hedefimiz, kullanıcıları sadece metinlerle bilgilendirmek değil, görsel bir anlatı ve etkileşimli bir arayüz ile tehlikenin farkına varmalarını sağlamaktır.

---

## 📢 SUNUM HAFTASI RAPORU: BU HAFTA NELERİ BAŞARDIK?
"Sunum Haftası" kapsamında projemiz, statik bir yapıdan profesyonel bir web platformuna evrilmiştir. Bu hafta odaklandığımız ana başlıklar şunlardır:

### 1. Görsel Derinlik ve Estetik (CSS3)
* **W3Schools Parallax Tekniği:** Sayfalarımızda `background-attachment: fixed;` özelliğini kullanarak, metinler kayarken arka planın sabit kaldığı modern bir derinlik algısı yarattık.
* **Renk Psikolojisi:** Bağımlılığın karanlık dünyasını yansıtan koyu gri/siyah tonları ile dikkat çekici uyarı kırmızısını (#e74c3c) birleştirdik.

### 2. İnteraktif "Sorunlar" Çizelgesi (Timeline)
* **Düz Çizgi Üzerinde Anlatım:** "Sorunlar" sayfasını tamamen yeniledik. Bağımlılığın **Ekonomik, Psikolojik, Akademik ve Sosyal** evrelerini dikey bir çizgi üzerinde sağlı-sollu akan bir kronoloji ile sunduk. Bu yapı sayesinde karmaşık bilgiler çok daha okunabilir hale getirildi.

### 3. Kod Optimizasyonu ve Duyarlılık
* Tüm sayfalar için merkezi bir `style.css` dosyası oluşturuldu.
* **Flexbox** yapısı kullanılarak sitenin mobil cihazlarda ve tabletlerde bozulmadan çalışması sağlandı.

---

## 🛠️ TEKNİK MİMARİ VE STANDARTLAR

Projemiz, modern web geliştirme pratiklerini ve W3Schools eğitim materyallerini referans alır:

### **Dinamik Arka Plan Yönetimi**
Görsellerin okunabilirliği bozmaması için CSS ile "Overlay" (Karartma) katmanı eklendi:
```css
/* Görsel üzerine transparan maske uygulaması */
#banner {
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('images/bg.jpg');
    background-size: cover;
    background-attachment: fixed; /* Parallax Etkisi */
}
