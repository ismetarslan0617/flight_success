<h1 align="center">MODEL ROKET UÇUŞLARI İÇİN DİJİTAL İKİZ YAKLAŞIMIYLA GELİŞTİRİLMİŞ DÜŞME BÖLGESİ TAHMİNİ VE ATIŞ ZAMANI/BÖLGESİ ÖNERİ SİSTEMİ</h1>
<h2 align="center">“Klasik simülasyon araçlarının deterministik yapısına karşı, dijital ikiz yaklaşımlı akıllı tahminler...”</h2>

<hr>

<h2 align="center">🎯 Amaç</h2>

<p align="center">
Lisans bitirme projesi olarak geliştirme aşamasına başlanan ve TÜBİTAK 2209-A Programı tarafından desteklenmeye hak kazanan bu projede amaç hava durumu parametrelerini kullanarak<br>
uçuşun <strong>başarılı / başarısız</strong> durumuyla birlikte <strong>düşme bölgesini</strong> tahmin etmek<br>
ve <strong>karar destek</strong> amacıyla yorumlanabilir sonuçlar üretmektir.
</p>

<hr>

<h2 align="center">🛠 Kullanılan Teknolojiler</h2>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Programming-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Pandas-Data%20Processing-150458?style=for-the-badge">
  <img src="https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?style=for-the-badge">
  <img src="https://img.shields.io/badge/Bayesian%20Network-Probabilistic%20Modeling-6A1B9A?style=for-the-badge">
</p>

<hr>

<h2 align="center">📊 Kullanılan Girdi Parametreleri</h2>

<p align="center">
Rüzgar Hızı (km/sa) • Sıcaklık (°C) • Nem (%) • Yağmur Olasılığı (%)
</p>

<hr>

<h2 align="center">🧭 Yöntem ve Süreç</h2>

<table align="center" width="100%">
  <tr>
    <td align="center">
      <h3>1️⃣ Veri Hazırlama</h3>
      <sub>
        Ham hava durumu verilerinin okunması,<br>
        eksik ve tutarsız verilerin temizlenmesi
      </sub>
    </td>
    <td align="center">
      <h3>2️⃣ Özellik Seçimi</h3>
      <sub>
        Rüzgar, sıcaklık, nem ve yağmur<br>
        parametrelerinin belirlenmesi
      </sub>
    </td>
    <td align="center">
      <h3>3️⃣ Etiketleme</h3>
      <sub>
        Uçuş başarısı (%) eşiklenerek<br>
        başarılı / başarısız sınıflarının oluşturulması
      </sub>
    </td>
  </tr>
</table>

<br>

<table align="center" width="100%">
  <tr>
    <td align="center">
      <h3>4️⃣ Model Eğitimi</h3>
      <sub>
        Farklı makine öğrenmesi<br>
        algoritmalarının eğitilmesi
      </sub>
    </td>
    <td align="center">
      <h3>5️⃣ Değerlendirme</h3>
      <sub>
        Accuracy, Confusion Matrix<br>
        ve karşılaştırmalı analiz
      </sub>
    </td>
    <td align="center">
      <h3>6️⃣ Karar Destek</h3>
      <sub>
        Yeni günler için tahmin,<br>
        olasılıksal risk analizi
      </sub>
    </td>
  </tr>
</table>

<hr>

<h2 align="center">🧠 Model Yaklaşımları</h2>

<table align="center" width="100%">
  <tr>
    <td align="center">
      <h3>🌲 Random Forest</h3>
      <sub>
        Ansambl tabanlı sınıflandırma,<br>
        gürültüye dayanıklı yapı
      </sub>
    </td>
    <td align="center">
      <h3>📈 Lojistik Regresyon</h3>
      <sub>
        Basit ve yorumlanabilir,<br>
        referans model
      </sub>
    </td>
     <td align="center">
      <h3>📐 Bayesian Network</h3>
      <sub>
        Olasılıksal yaklaşım,<br>
        koşullu başarı analizi
      </sub>
    </td>
  </tr>
</table>

<br>

<hr>

<h2 align="center">📋 Örnek Model Çıktıları (Head)</h2>

<p align="center">
Aşağıda, eğitilmiş modellerin yeni hava durumu verileri üzerindeki
<strong>ilk tahmin çıktıları</strong> yer almaktadır.
</p>

<h3 align="center">🌲 Random Forest – Sınıflandırma Çıktısı</h3>

<table align="center" border="1" cellpadding="6">
  <tr>
    <th>Rüzgar</th>
    <th>Sıcaklık</th>
    <th>Nem</th>
    <th>Yağmur</th>
    <th>Tahmin</th>
  </tr>
  <tr>
    <td align="center">12</td>
    <td align="center">18</td>
    <td align="center">55</td>
    <td align="center">10</td>
    <td align="center"><strong>Başarılı</strong></td>
  </tr>
  <tr>
    <td align="center">28</td>
    <td align="center">14</td>
    <td align="center">80</td>
    <td align="center">60</td>
    <td align="center"><strong>Başarısız</strong></td>
  </tr>
</table>

<br>

<h3 align="center">📐 Bayesian Network – Olasılıksal Çıktı</h3>

<table align="center" border="1" cellpadding="6">
  <tr>
    <th>Koşul</th>
    <th>Başarılı Olasılığı</th>
    <th>Başarısız Olasılığı</th>
  </tr>
  <tr>
    <td align="center">Düşük Rüzgar</td>
    <td align="center">0.78</td>
    <td align="center">0.22</td>
  </tr>
  <tr>
    <td align="center">Yüksek Yağmur</td>
    <td align="center">0.18</td>
    <td align="center">0.82</td>
  </tr>
</table>

<p align="center">
<sub>
Tablolar, çıktı dosyalarının ilk satırlarını (head) temsil etmektedir.
Sunum sırasında model davranışını gözlemlemek amacıyla kullanılmıştır.
</sub>
</p>

<hr>

<h2 align="center">📌 Proje Notu</h2>

<p align="center">
Model çıktıları, <strong>sunum sırasında iki taraflı gözlem</strong> yapılabilmesi için<br>
eğitim verisi ve yeni (365 günlük) veri üzerinde ayrı ayrı incelenmiştir.<br>
Bazı veri alt kümeleri <strong>sunum kolaylığı</strong> amacıyla seçilmiştir.
</p>

<hr>

<h2 align="center">🚀 Geliştirici</h2>

<p align="center">
<strong>İsmet Arslan</strong><br>
Bilgisayar Mühendisliği Öğrencisi<br>
Makine Öğrenmesi • Veri İşleme • Karar Destek Sistemleri
</p>
