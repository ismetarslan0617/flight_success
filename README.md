<hr>

<h2 align="center">📋 Örnek Model Çıktıları (Head)</h2>

<p align="center">
Aşağıda, eğitilmiş modellerin yeni hava durumu verileri üzerindeki
<strong>ilk tahmin çıktıları</strong> yer almaktadır.
</p>

<h3 align="center">🌲 Random Forest – Sınıflandırma Çıktısı</h3>

<table align="center" border="1" cellpadding="6">
  <tr>
    <th>Rüzgar (km/sa)</th>
    <th>Sıcaklık (°C)</th>
    <th>Nem (%)</th>
    <th>Yağmur (%)</th>
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
  <tr>
    <td align="center">20</td>
    <td align="center">22</td>
    <td align="center">65</td>
    <td align="center">30</td>
    <td align="center"><strong>Başarılı</strong></td>
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
    <td align="center">Orta Nem</td>
    <td align="center">0.55</td>
    <td align="center">0.45</td>
  </tr>
  <tr>
    <td align="center">Yüksek Yağmur</td>
    <td align="center">0.18</td>
    <td align="center">0.82</td>
  </tr>
</table>

<p align="center">
<sub>
Tablolarda yer alan değerler, çıktı dosyalarının ilk satırlarını (head) temsil etmektedir.
Sunum sırasında model davranışının daha net gözlemlenebilmesi amacıyla kullanılmıştır.
</sub>
</p>
