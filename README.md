<h1 align="center">🌦️ Hava Durumu Tabanlı Uçuş Başarı Tahmini</h1>
<h2 align="center">Makine Öğrenmesi ile Karar Destek Sistemi</h2>

<hr>

<h2 align="center">🎯 Amaç</h2>

<p align="center">
Hava durumu parametrelerini kullanarak<br>
uçuşun <strong>başarılı / başarısız</strong> olacağını tahmin etmek<br>
ve <strong>karar destek</strong> amacıyla yorumlanabilir sonuçlar üretmek.
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

<p align="center">
  <img src="https://img.shields.io/badge/Random%20Forest-ensemble-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Logistic%20Regression-interpretable-informational?style=for-the-badge" />
  <img src="https://img.shields.io/badge/KNN-similarity-blue?style=for-the-badge" /><br>
  <img src="https://img.shields.io/badge/SVM-margin%20based-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Bayesian%20Network-probabilistic-6A1B9A?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Naive%20Bayes-fast-lightgrey?style=for-the-badge" />
</p>

<details>
  <summary><strong>🌲 Random Forest</strong> — Gürültüye dayanıklı ansambl</summary>
  <br>
  <ul>
    <li>Birden fazla karar ağacının oylamasıyla çalışır.</li>
    <li>Gürültü/outlier etkisine nispeten dayanıklıdır.</li>
    <li>Yeni gün verilerinde tahmin için ana model olarak kullanılır.</li>
  </ul>
</details>

<details>
  <summary><strong>📈 Lojistik Regresyon</strong> — Basit ve yorumlanabilir referans</summary>
  <br>
  <ul>
    <li>Doğrusal karar sınırı üretir.</li>
    <li>“Hangi parametre ne kadar etkili?” anlatımını güçlendirir.</li>
  </ul>
</details>

<details>
  <summary><strong>📊 KNN</strong> — Benzer günlere göre tahmin</summary>
  <br>
  <ul>
    <li>“Benzer hava koşulları → benzer sonuç” mantığıyla çalışır.</li>
    <li>Ölçekleme (scaling) ve k seçimine duyarlıdır.</li>
  </ul>
</details>

<details>
  <summary><strong>⚙️ SVM</strong> — Güçlü karar sınırları</summary>
  <br>
  <ul>
    <li>Marjin maksimize ederek sınıfları ayırır.</li>
    <li>Kernel ile doğrusal olmayan ayrım yapabilir.</li>
  </ul>
</details>

<details>
  <summary><strong>📐 Bayesian Network</strong> — Olasılıksal karar destek</summary>
  <br>
  <ul>
    <li>Koşullu olasılıklarla “şu koşulda başarı olasılığı kaç?” sorusunu cevaplar.</li>
    <li>Yorumlanabilirlik (explainability) için güçlüdür.</li>
  </ul>
</details>

<details>
  <summary><strong>🧮 Naive Bayes</strong> — Hızlı ve hafif</summary>
  <br>
  <ul>
    <li>Özellik bağımsızlığı varsayımıyla hızlı tahmin yapar.</li>
    <li>Baseline karşılaştırma için idealdir.</li>
  </ul>
</details>

<hr>

<h2 align="center">📋 Örnek Model Çıktıları (Head)</h2>

<p align="center">
  Aşağıda, yeni hava durumu verileri üzerindeki <strong>ilk tahmin çıktıları</strong> örneklenmiştir.
</p>

<h3 align="center">🌲 Random Forest — Sınıflandırma Çıktısı</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Tahminler-Head%20Preview-2ea44f?style=for-the-badge" />
</p>

<table align="center">
  <tr>
    <th>Rüzgar</th><th>Sıcaklık</th><th>Nem</th><th>Yağmur</th><th>Tahmin</th>
  </tr>
  <tr>
    <td align="center">12</td><td align="center">18</td><td align="center">55</td><td align="center">10</td>
    <td align="center">✅ <strong>Başarılı</strong></td>
  </tr>
  <tr>
    <td align="center">28</td><td align="center">14</td><td align="center">80</td><td align="center">60</td>
    <td align="center">❌ <strong>Başarısız</strong></td>
  </tr>
</table>

<br>

<h3 align="center">📐 Bayesian Network — Olasılıksal Çıktı</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Koşullu%20Olasılıklar-Head%20Preview-6A1B9A?style=for-the-badge" />
</p>

<table align="center">
  <tr>
    <th>Koşul</th><th>Başarılı</th><th>Başarısız</th>
  </tr>
  <tr>
    <td align="center">Düşük Rüzgar</td><td align="center">0.78</td><td align="center">0.22</td>
  </tr>
  <tr>
    <td align="center">Yüksek Yağmur</td><td align="center">0.18</td><td align="center">0.82</td>
  </tr>
</table>

<p align="center">
  <sub>Not: Tablolar çıktı dosyalarının ilk satırlarını (head) temsil eder; sunumda model davranışını hızlı gözlemlemek için kullanılır.</sub>
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
