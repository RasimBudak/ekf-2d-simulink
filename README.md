# 2D EKF (Extended Kalman Filter) Simulink Uygulaması

Bu proje, MATLAB Simulink kullanılarak geliştirilen 2 boyutlu bir **Extended Kalman Filter (EKF)** uygulamasıdır.

## 📌 Amaç

- Gürültülü konum ölçümlerinden (z_x, z_y), EKF kullanarak [x, y, vx, vy] durumlarının tahmini
- Simulink ortamında sistem modelleme ve filtreleme simülasyonu

## 🛠️ Kullanılan Yapılar

- `Integrator` blokları ile gerçek konum oluşturulması
- `Random Number` blokları ile gürültü eklenmesi
- `MATLAB Function` bloğu içinde 2D EKF algoritması
- `Scope` blokları ile x/y konum ve hız tahminlerinin gözlemi

## 📊 Sonuç

Model, 2D uzayda hareket eden bir nesnenin pozisyonunu ve hızını tahmin etmektedir. Aşağıda örnek çıktı grafikleri yer almaktadır:

![EKF Scope Çıktısı](media/ekran_goruntusu.png)

## 🚀 Simülasyon Ayarları

- Solver: `Fixed-step`, Euler (`ode1`)
- Step size: `0.1`
- Stop time: `30`

## 📁 Dosyalar

- `ekf_2d.slx`: Simulink model dosyası
- `media/`: Ekran görüntüleri ve medya
