# Derin Beyin Stimülasyonu (DBS) Sonrası İyileşme ve Optimal Süreye Ulaşma

## Kapsamlı Araştırma Dökümanı

---

## İçindekiler

1. [DBS Nedir?](#1-dbs-nedir)
2. [DBS Cerrahi Prosedürü](#2-dbs-cerrahi-prosedürü)
3. [Post Operatif İyileşme Süreci](#3-post-operatif-iyileşme-süreci)
4. [Programlama ve Optimizasyon Süreci](#4-programlama-ve-optimizasyon-süreci)
5. [Klinik Sonuçlar ve İyileşme Verileri](#5-klinik-sonuçlar-ve-iyileşme-verileri)
6. [Hastalık Bazlı İyileşme Süreleri](#6-hastalık-bazlı-iyileşme-süreleri)
7. [Rehabilitasyon ve Fizik Tedavi](#7-rehabilitasyon-ve-fizik-tedavi)
8. [Optimal Süreyi Etkileyen Faktörler](#8-optimal-süreyi-etkileyen-faktörler)
9. [Makine Öğrenmesi ve Optimizasyon Modelleri](#9-makine-öğrenmesi-ve-optimizasyon-modelleri)
10. [Veri Özeti ve Model Parametreleri](#10-veri-özeti-ve-model-parametreleri)

---

## 1. DBS Nedir?

Derin Beyin Stimülasyonu (DBS), beynin belirli bölgelerine implante edilen elektrotlar aracılığıyla kontrollü elektrik impulsleri gönderen bir nörostimülasyon tedavisidir. İmplante edilebilir bir puls jeneratörü (IPG) göğüs derisi altına yerleştirilir ve beyne uzanan elektrotlara bağlanır.

### 1.1 Endikasyonlar

| Hastalık | FDA Onayı | Hedef Bölge | Başarı Oranı |
|----------|-----------|-------------|--------------|
| Parkinson Hastalığı | Evet | STN / GPi | %50-90 |
| Esansiyel Tremor | Evet | VIM | %50-70 |
| Distoni | Evet | GPi | %45-60 |
| Epilepsi | Evet | ATN | %56 |
| OKB | HDE | VC/VS | Değişken |

**Kısaltmalar:**
- STN: Subthalamik Nükleus
- GPi: Globus Pallidus Interna
- VIM: Ventral İntermediat Nükleus
- ATN: Anterior Thalamik Nükleus
- HDE: Humanitarian Device Exemption

### 1.2 DBS Mekanizması

DBS, beyinde anormal şekilde artmış ve aşırı uyumlu hâle gelmiş sinirsel aktiviteleri baskılayarak etki gösterir. Mekanizması henüz tüm ayrıntılarıyla açıklanamamış olsa da, hedeflenen bölgede oluşturulan kontrollü bir işlevsel “kesinti” ile lezyonlama etkisine benzer bir sonuç doğurduğu düşünülmektedir.

---

## 2. DBS Cerrahi Prosedürü

### 2.1 Pre-Operatif Değerlendirme

Pre-operatif değerlendirme süreci tipik olarak birkaç ay sürer ve şunları içerir:

1. **Nörolojik Değerlendirme**
   - UPDRS (Unified Parkinson's Disease Rating Scale) skorlaması
   - Levodopa challenge testi
   - Motor fluktuasyonların değerlendirilmesi

2. **Nöropsikolojik Testler**
   - Kognitif fonksiyon değerlendirmesi
   - Demans taraması
   - Depresyon ve anksiyete taraması

3. **Görüntüleme**
   - Yüksek çözünürlüklü MRI (1mm kesit kalınlığı)
   - FGATIR sekansları (bazal ganglion delineasyonu için)
   - CT tarama (stereotaktik planlama için)

4. **Medikal Değerlendirme**
   - Genel sağlık durumu
   - Kardiyovasküler değerlendirme
   - Koagülasyon profili

### 2.2 Cerrahi Teknikler

| Teknik | Anestezi | Süre | Avantajlar | Dezavantajlar |
|--------|----------|------|------------|---------------|
| Uyanık DBS | Lokal | 4-6 saat | Gerçek zamanlı test | Hasta konforu düşük |
| Uyku DBS | Genel | 3-5 saat | Hasta konforu yüksek | Gerçek zamanlı test yok |
| Aşamalı Cerrahi | Her ikisi | 2 seans | Risk dağılımı | Uzun toplam süre |

**Cerrahi Adımlar:**

1. **Stereotaktik Çerçeve Yerleştirme** (veya çerçevesiz navigasyon)
2. **Kranyal Marker Yerleştirme** - Lokal anestezi ile, 4 marker
3. **CT/MRI Füzyon** - Hedef koordinatların belirlenmesi
4. **Burr Hole Açılması** - ~14mm çap
5. **Elektrot İmplantasyonu** - Mikroelektrot kaydı ile
6. **İntra-operatif Test Stimülasyonu**
7. **Kalıcı Elektrot Fiksasyonu**
8. **IPG İmplantasyonu** - Göğüs duvarı, klavikula altı

### 2.3 Cerrahi Hedefler ve Koordinatlar

**Parkinson Hastalığı için STN Koordinatları:**
- Lateral: AC-PC hattından 11-12mm
- Anterior: PC'nin 3-4mm anterioru
- Inferior: AC-PC hattının 4-5mm altı

---

## 3. Post-Operatif İyileşme Süreci

### 3.1 İyileşme Zaman Çizelgesi

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    DBS SONRASI İYİLEŞME ZAMÂNCETVELİ                    │
├─────────────┬───────────────────────────────────────────────────────────┤
│ Dönem       │ Süreç ve Beklentiler                                      │
├─────────────┼───────────────────────────────────────────────────────────┤
│ 0-24 saat   │ - Yoğun bakım gözlemi                                     │
│             │ - Post-op CT (elektrot yerleşimi, kanama kontrolü)        │
│             │ - Vital bulguların monitörizasyonu                        │
├─────────────┼───────────────────────────────────────────────────────────┤
│ 1-3 gün     │ - Hastane yatışı (ortalama 1-2 gün)                       │
│             │ - İnsizyonların değerlendirilmesi                         │
│             │ - Erken mobilizasyon                                      │
│             │ - "Honeymoon etkisi" başlangıcı (mikrolezyon etkisi)      │
├─────────────┼───────────────────────────────────────────────────────────┤
│ 1-2 hafta   │ - Eve taburcu                                         │
│             │ - Yara bakımı                                             │
│             │ - Aktivite kısıtlamaları (ağır kaldırma yasak)            │
│             │ - Araç kullanma yasağı                                    │
├─────────────┼───────────────────────────────────────────────────────────┤
│ 2-4 hafta   │ - İlk programlama seansı                                  │
│             │ - Cihaz aktivasyonu                                       │
│             │ - Başlangıç stimülasyon ayarları                          │
│             │ - "Honeymoon etkisi" sonlanması                           │
├─────────────┼───────────────────────────────────────────────────────────┤
│ 1-3 ay      │ - Yoğun programlama dönemi                                │
│             │ - Çoklu klinik vizitler (haftalık/2 haftada bir)          │
│             │ - İlaç doz ayarlamaları                                   │
│             │ - Yan etkilerin yönetimi                                  │
├─────────────┼───────────────────────────────────────────────────────────┤
│ 3-6 ay      │ - Optimal ayarlara ulaşma                                 │
│             │ - İlaç azaltımı                                           │
│             │ - Motor fonksiyonlarda belirgin düzelme                   │
│             │ - Yaşam kalitesi iyileşmesi                               │
├─────────────┼───────────────────────────────────────────────────────────┤
│ 6-12 ay     │ - Stabilizasyon dönemi                                    │
│             │ - Periyodik kontroller (3-6 ayda bir)                     │
│             │ - İnce ayar düzenlemeleri                                 │
│             │ - Tam adaptasyon                                          │
├─────────────┼───────────────────────────────────────────────────────────┤
│ >12 ay      │ - Uzun vadeli takip                                       │
│             │ - Yıllık kontroller                                       │
│             │ - Batarya durumu takibi                                   │
│             │ - Gerektiğinde re-programlama                             │
└─────────────┴───────────────────────────────────────────────────────────┘
```

### 3.2 Erken Post-Operatif Dönem (0-4 Hafta)

**Beklenen Bulgular:**
- Göz çevresi şişlik (1-2 hafta)
- İnsizyon hassasiyeti
- Hafif baş ağrısı
- Geçici konfüzyon (%5.4-26.5)

**Dikkat Edilmesi Gereken Komplikasyonlar:**

| Komplikasyon | Görülme Sıklığı | Acil Müdahale Gerektirir |
|--------------|----------|--------------------------|
| İntrakranyal kanama | %2.3 (tümü), %0.7 (majör) | Evet |
| Enfeksiyon | %3-6 | Evet |
| Post-op delirium | %5.4-26.5 | Değerlendirmeye bağlı |
| Nöbet | <%1 | Evet |
| Mortalite | %0.26 (genel), %0.032 (PD) | - |

**Aktivite Kısıtlamaları:**
- İlk 2 hafta: Minimal aktivite
- İlk 4-6 hafta: 5-10 kg'dan fazla ağırlık kaldırmama
- İlk 2 hafta: Araç kullanmama, uçuş yasağı

### 3.3 "Honeymoon Etkisi"

Cerrahiden hemen sonra, cihaz henüz aktive edilmeden önce bile semptomlarda geçici iyileşme görülebilir. Bu etki:

- **Nedeni:** Elektrot implantasyonu sırasında oluşan mikrolezyon
- **Süresi:** Genellikle 2-4 hafta
- **Önemi:** Bu dönemde ilaç değişikliği yapılmamalı
- **Dikkat:** Geçici bir etki olduğu hasta ve yakınlarına anlatılmalı

---

## 4. Programlama ve Optimizasyon Süreci

### 4.1 Programlama Parametreleri

DBS programlaması 4 temel parametrenin ayarlanmasını içerir:

| Parametre | Aralık | Tipik Başlangıç | Optimum |
|-----------|--------|-----------------|---------|
| Amplitüd (Voltaj/Akım) | 0-10.5V / 0-25.5mA | 1.0-2.0V | Bireysel |
| Puls Genişliği | 30-450 μs | 60-90 μs | 60-90 μs |
| Frekans | 2-250 Hz | 130-185 Hz | 130-185 Hz |
| Elektrot Konfigürasyonu | Monopolar/Bipolar | Monopolar | Bireysel |

### 4.2 Programlama Yaklaşımları

**1. Konvansiyonel Klinik Programlama (CP)**
- Altın standart
- Her kontak tek tek test edilir
- Klinik yanıt ve yan etkiler değerlendirilir
- **Süre:** 45-60 dakika/seans
- **Dezavantaj:** Zaman yoğun, çoklu vizit gerektirir

**2. Görüntü Kılavuzluğunda Programlama (IGP)**
- Post-op görüntüleme kullanılır
- Stimülasyon alanı 3D olarak modellenir
- **Süre:** ~20 dakika/seans
- **Sonuç:** %83.9 hastada motor ve yaşam kalitesi iyileşmesi
- **Avantaj:** Programlama süresini %57 azaltır

**3. Beta-Kılavuzluğunda Programlama**
- STN'den yerel alan potansiyelleri (LFP) kaydedilir
- Beta band (13-30 Hz) gücü biomarker olarak kullanılır
- Klinik programlamaya eşdeğer etkinlik
- Önemli ölçüde daha kısa süre

**4. Uzaktan Programlama**
- Mobil uygulama üzerinden ayar değişikliği
- Daha hızlı semptom iyileşmesi
- Klinik vizit sayısını azaltır

### 4.3 Optimal Ayarlara Ulaşma Süresi

```
┌──────────────────────────────────────────────────────────────┐
│           OPTİMAL PROGRAMLAMAYA ULAŞMA SÜRESİ               │
├──────────────────────────────────────────────────────────────┤
│                                                              │
│   Başlangıç ────▶ 2-4 hafta: İlk programlama                │
│                              ↓                               │
│              ────▶ 4-6 hafta: İkinci ayarlama                │
│                              ↓                               │
│              ────▶ 6-9 hafta: İnce ayar                      │
│                              ↓                               │
│              ────▶ 3 ay: Optimal ayarların %60-70'i         │
│                              ↓                               │
│              ────▶ 6 ay: Optimal ayarların %80-90'ı         │
│                              ↓                               │
│              ────▶ 12 ay: Tam optimizasyon                   │
│                                                              │
│   Ortalama Programlama Seansı: 3-6 seans                    │
│   Ortalama Optimizasyon Süresi: 3-6 ay                      │
│   Minimum Seans Sayısı: 3 (nadir)                           │
│                                                              │
└──────────────────────────────────────────────────────────────┘
```

### 4.4 Programlama Seanslarının Zamanlaması

| Seans | Zamanlama | Amaç |
|-------|-----------|------|
| 1 | 2-4 hafta | Cihaz aktivasyonu, başlangıç ayarları |
| 2 | 4-6 hafta | İnce ayar, yan etki yönetimi |
| 3 | 6-9 hafta | Optimizasyon |
| 4 | 3 ay | Değerlendirme, ilaç ayarlaması |
| 5 | 6 ay | Uzun vadeli ayarlama |
| 6+ | Gerektiğinde | İdame, batarya kontrolü |

---

## 5. Klinik Sonuçlar ve İyileşme Verileri

### 5.1 Parkinson Hastalığı - UPDRS İyileşme Oranları

**Kısa Vadeli Sonuçlar (6-12 ay):**

| Parametre | STN-DBS | GPi-DBS | Kaynak |
|-----------|---------|---------|--------|
| UPDRS-III (Motor) iyileşme | %50.5 | %29.8 | Meta-analiz (2021) |
| UPDRS-II (ADL) iyileşme | %47 | %18.5 | Meta-analiz (2021) |
| Diskinezi azalması | %60-80 | %60-80 | Çoklu çalışma |
| OFF periyodu azalması | %68 | - | Sistemik derleme |
| LEDD (ilaç dozu) azalması | %56 | %10-20 | Karşılaştırmalı çalışma |
| Yaşam kalitesi iyileşmesi | %35 | %30 | Sistemik derleme |

**MDS-UPDRS Detaylı İyileşme (6 ay sonrası):**

| Alt Bölüm | İyileşme | Yüzde |
|-----------|----------|-------|
| Part I (Non-motor) | 3.1 puan | %22 |
| Part II (ADL) | 5.3 puan | %29 |
| Part III (Motor) | 13.1 puan | %29 |
| Part IV (Komplikasyonlar) | 7.1 puan | %74 |

**Spesifik Semptom İyileşmeleri (1 yıl sonrası):**

| Semptom | İyileşme Oranı |
|---------|----------------|
| Tremor | %80 |
| Rijidite | %58 |
| Bradikinezi | %53 |
| Yürüyüş | %52 |
| Postural instabilite | %50 |

### 5.2 Uzun Vadeli Sonuçlar

**8-15 Yıllık Takip Verileri:**

| Zaman | Motor UPDRS İyileşmesi (stimülasyon ON) |
|-------|----------------------------------------|
| 1 yıl | %61 |
| 8-15 yıl | %39 |
| Re-programlama sonrası | %45-50 |

**15+ Yıllık Sonuçlar:**
- Diskinezi süresi: %75 azalma
- OFF durumunda geçen süre: %58.7 azalma
- Dopaminerjik ilaç kullanımı: %50.6 azalma
- Yaşam kalitesi: Korunmuş veya iyileşmiş

### 5.3 Hastalık Bazlı İyileşme Süreleri

**Parkinson Hastalığı:**
- İlk iyileşme: Programlama sonrası saatler-günler içinde
- Optimal fayda: 3-6 ay
- Stabil dönem: 6-12 ay

**Esansiyel Tremor:**
- İlk iyileşme: Dakikalar içinde
- Optimal fayda: 1-3 ay
- **Dikkat:** Uzun vadede habitüasyon riski

**Distoni:**
- İlk iyileşme: Haftalar-aylar
- Optimal fayda: 6-12 ay
- **Gecikme nedeni:** Nöroplastik yeniden modelleme gereksinimi

**Epilepsi:**
- Medyan nöbet azalması: %56 (2 yıl içinde)
- Progresif iyileşme: Zamanla artar

---

## 6. Hastalık Bazlı İyileşme Süreleri

### 6.1 Parkinson Hastalığı Detaylı Zaman Çizelgesi

```
Hafta 0-2:   ▓░░░░░░░░░░░░░░░░░░░░░░░░░ Honeymoon etkisi
Hafta 2-4:   ▓▓░░░░░░░░░░░░░░░░░░░░░░░░ İlk programlama
Hafta 4-6:   ▓▓▓░░░░░░░░░░░░░░░░░░░░░░░ Erken yanıt
Ay 2-3:      ▓▓▓▓▓░░░░░░░░░░░░░░░░░░░░░ Belirgin iyileşme
Ay 3-6:      ▓▓▓▓▓▓▓▓░░░░░░░░░░░░░░░░░░ Optimizasyon
Ay 6-12:     ▓▓▓▓▓▓▓▓▓▓░░░░░░░░░░░░░░░░ Stabilizasyon
Yıl 1-5:     ▓▓▓▓▓▓▓▓▓▓▓▓░░░░░░░░░░░░░░ İdame
Yıl 5+:      ▓▓▓▓▓▓▓▓▓▓▓▓▓▓░░░░░░░░░░░░ Uzun vadeli takip
```

### 6.2 Esansiyel Tremor

| Dönem | Tremor Azalması | Fonksiyonel İyileşme |
|-------|-----------------|----------------------|
| Hemen | %50-70 | Değişken |
| 6 ay | %70-80 | %56 |
| 1 yıl | %65-75 | %50-56 |
| 2+ yıl | %50-65 | Azalabilir |

**Önemli:** VIM-DBS'de uzun vadede etkinlik kaybı (habitüasyon) görülebilir. Bir çalışmada 10 yıl içinde etkinliğin ciddi şekilde azaldığı gösterilmiştir.

### 6.3 Distoni

| Distoni Tipi | GPi-DBS İyileşme | Optimal Süre |
|--------------|------------------|--------------|
| Primer jeneralize | %45-60 | 6-12 ay |
| Servikal | %40-70 | 6-12 ay |
| Segmental | %40-50 | 6-12 ay |
| Sekonder | Değişken | 12+ ay |

**Gecikmiş Yanıt Nedenleri:**
- Distonik motor devrelerinin karmaşıklığı
- Uzun vadeli nöroplastik yeniden modelleme gerekliliği
- Nöral adaptasyon süreci

---

## 7. Rehabilitasyon ve Fizik Tedavi

### 7.1 DBS Sonrası Fizik Tedavi Önerileri

Uzman konsensüsü, DBS sonrası konvansiyonel fizik tedavinin önerildiğini göstermektedir:

**Rehabilitasyon Hedefleri:**
1. Postural stabilite iyileştirme
2. Yürüyüş performansı geliştirme
3. Donma (freezing) semptomlarını azaltma
4. Fonksiyonel kapasite artırma
5. Düşme riskini azaltma

### 7.2 Egzersiz Programı Bileşenleri

| Bileşen | Süre | Frekans | Yoğunluk |
|---------|------|---------|----------|
| Isınma | 5-10 dk | Her seans | Düşük |
| Aerobik egzersiz | 20-30 dk | 3-5x/hafta | Orta-yüksek |
| Güç antrenmanı | 15-20 dk | 2-3x/hafta | Progresif |
| Denge egzersizleri | 10-15 dk | Günlük | Bireysel |
| Postüral egzersizler | 10 dk | Günlük | Düşük-orta |
| Proprioseptif aktiviteler | 10 dk | 3x/hafta | Bireysel |

### 7.3 Kanıta Dayalı Rehabilitasyon Sonuçları

**Parkinson's Outcomes Project Bulguları:**
- Haftada 2.5 saat egzersiz yapanlar yaşam kalitesinde daha yavaş düşüş gösteriyor
- Erken başlanan egzersiz programları daha iyi sonuçlar veriyor

**DBS + Rehabilitasyon Kombinasyonu:**
- UPDRS skorlarında iyileşme
- Berg Denge Skalasında iyileşme
- 6 Dakika Yürüme Testinde artış
- TUG (Timed Up and Go) testinde azalma

### 7.4 Rehabilitasyon Zamanlaması

| Dönem | Rehabilitasyon Odağı |
|-------|----------------------|
| 0-2 hafta | Erken mobilizasyon, hafif aktivite |
| 2-6 hafta | Progresif yürüyüş programı |
| 6-12 hafta | Kapsamlı rehabilitasyon başlangıcı |
| 3-6 ay | Yoğun egzersiz programı |
| 6+ ay | İdame egzersiz programı |

---

## 8. Optimal Süreyi Etkileyen Faktörler

### 8.1 Pozitif Prediktörler (Daha Hızlı/İyi İyileşme)

| Faktör | Etki | Kanıt Düzeyi |
|--------|------|--------------|
| Genç yaş (<60) | Daha iyi uzun vadeli sonuçlar | Yüksek |
| İyi levodopa yanıtı (>%30 UPDRS) | Daha iyi DBS yanıtı | Yüksek |
| Kısa hastalık süresi | Daha iyi sonuçlar | Orta |
| Korunmuş kognitif fonksiyon | Daha güvenli prosedür | Yüksek |
| Yüksek volüm merkez | Daha iyi cerrahi sonuçlar | Yüksek |
| Deneyimli programlama ekibi | Daha hızlı optimizasyon | Yüksek |
| Doğru elektrot yerleşimi | Optimal tedavi | Çok yüksek |

### 8.2 Negatif Prediktörler (Daha Yavaş/Zor İyileşme)

| Faktör | Risk | Kanıt Düzeyi |
|--------|------|--------------|
| İleri yaş (>70) | Uzun hastane kalışı | Yüksek |
| Kognitif bozukluk | Sınırlı fayda | Yüksek |
| Sık düşme öyküsü | Uzun iyileşme | Orta |
| Ağır aksiyel semptomlar | Sınırlı iyileşme | Orta |
| Kardiyovasküler komorbidite | Artan komplikasyon riski | Orta |
| Obezite | Cerrahi komplikasyon riski | Orta |
| Psikiyatrik komorbidite | Değişken yanıt | Orta |

### 8.3 Cerrahi ve Teknik Faktörler

| Faktör | Optimal Koşul |
|--------|---------------|
| Elektrot yerleşimi | "Sweet spot" hedefleme |
| Cerrahi deneyim | >50 prosedür/yıl |
| Görüntüleme kalitesi | 3T MRI, ince kesit |
| İntra-operatif test | Mikro-elektrot kaydı + test stimülasyonu |

### 8.4 Optimal Süreyi Hesaplama Modeli

**Temel Formül (Konseptüel):**

```
Optimal_Süre = Baz_Süre + Σ(Risk_Faktörleri × Ağırlık) - Σ(Pozitif_Faktörler × Ağırlık)

Baz_Süre = 90 gün (Parkinson), 30 gün (ET), 180 gün (Distoni)
```

**Örnek Hesaplama (Parkinson Hastalığı):**

| Faktör | Değer | Ağırlık | Katkı (gün) |
|--------|-------|---------|-------------|
| Baz süre | - | - | +90 |
| Yaş >70 | Evet/Hayır | 0.3 | +30 |
| Kognitif bozukluk | Evet/Hayır | 0.4 | +45 |
| Düşme öyküsü | Evet/Hayır | 0.2 | +20 |
| IGP kullanımı | Evet/Hayır | -0.3 | -25 |
| Deneyimli merkez | Evet/Hayır | -0.2 | -15 |

---

## 9. Makine Öğrenmesi ve Optimizasyon Modelleri

### 9.1 Mevcut ML Uygulamaları

**1. fMRI Tabanlı Optimal Parametre Tahmini**
- **Yöntem:** fMRI yanıt paternleri + makine öğrenmesi
- **Doğruluk:** %88 (a priori optimize edilmiş hastalar)
- **Stimülasyon-naif hastalar:** %76 doğruluk
- **Model:** Linear Discriminant Analysis
- **Özellikler:** Motor korteks BOLD aktivasyonu

**2. Derin Öğrenme Tabanlı Programlama**
- **Yöntem:** Autoencoder + MLP
- **Sınıflandırma doğruluğu:** %96
- **Voltaj tahmini:** %79
- **Frekans tahmini:** %85
- **Kontak lokasyonu:** %70-83
- **Potansiyel:** TPP'yi 1 yıldan birkaç saate indirme

**3. Görüntü Kılavuzluğunda Programlama (IGP)**
- **Yöntem:** VTA (Volume of Tissue Activated) modelleme
- **Programlama süresi:** 19.78 ± 5.86 dk vs 45.22 ± 18.32 dk
- **Klinik sonuçlar:** Eşdeğer motor kontrol

**4. Random Forest Frekans Optimizasyonu**
- **Girdi:** Pre-operatif hasta ve hastalık özellikleri
- **Çıktı:** Optimal stimülasyon frekansı (yüksek vs 60 Hz)
- **Doğruluk:** %95

### 9.2 Model Geliştirme için Veri Gereksinimleri

**Minimum Veri Seti:**

| Veri Tipi | Minimum N | Önerilen N |
|-----------|-----------|------------|
| Demografik | 30 | 100+ |
| Pre-op UPDRS | 30 | 100+ |
| Elektrot koordinatları | 30 | 100+ |
| Stimülasyon parametreleri | 100 (seans) | 500+ |
| Post-op UPDRS | 30 | 100+ |
| fMRI (opsiyonel) | 20 | 50+ |

**Özellik Vektörü (Örnek):**

```python
features = {
    # Demografik
    'age': continuous,
    'gender': binary,
    'disease_duration': continuous,
    
    # Pre-operatif
    'updrs_off': continuous,
    'updrs_on': continuous,
    'levodopa_response': continuous,
    'led': continuous,
    'hoehn_yahr': ordinal,
    
    # Anatomik
    'electrode_x': continuous,
    'electrode_y': continuous,
    'electrode_z': continuous,
    'vta_volume': continuous,
    
    # Stimülasyon
    'voltage': continuous,
    'pulse_width': continuous,
    'frequency': continuous,
    'contact_config': categorical,
    
    # Hedef
    'optimal_time': continuous,  # gün cinsinden
    'final_updrs_improvement': continuous  # yüzde
}
```

### 9.3 Önerilen Model Mimarisi

**Model 1: Optimal Süre Tahmini (Regresyon)**

```
Girdi Katmanı (20 özellik)
    ↓
Dense Katman (64 nöron, ReLU)
    ↓
Dropout (0.3)
    ↓
Dense Katman (32 nöron, ReLU)
    ↓
Dropout (0.2)
    ↓
Dense Katman (16 nöron, ReLU)
    ↓
Çıkış Katmanı (1 nöron, Linear)
    ↓
Çıkış: Optimal süre (gün)
```

**Model 2: İyileşme Kategorisi Tahmini (Sınıflandırma)**

```
Girdi Katmanı (20 özellik)
    ↓
Dense Katman (128 nöron, ReLU)
    ↓
BatchNormalization
    ↓
Dense Katman (64 nöron, ReLU)
    ↓
Dropout (0.4)
    ↓
Dense Katman (32 nöron, ReLU)
    ↓
Çıkış Katmanı (3 nöron, Softmax)
    ↓
Çıkış: [Hızlı, Normal, Yavaş] iyileşme
```

---

## 10. Veri Özeti ve Model Parametreleri

### 10.1 Özet İstatistikler

**Global DBS Verileri:**
- Toplam DBS implantı (2019'a kadar): ~160,000
- Yıllık prosedür sayısı: ~12,000
- En yaygın endikasyon: Parkinson hastalığı

**İyileşme Süreleri Özeti:**

| Hastalık | Median Süre | Min | Max |
|----------|-------------|-----|-----|
| Parkinson (optimal) | 90-180 gün | 30 gün | 365 gün |
| Esansiyel tremor | 30-90 gün | 1 hafta | 180 gün |
| Distoni | 180-365 gün | 90 gün | 730 gün |
| Epilepsi | 180-730 gün | 90 gün | 1095 gün |

### 10.2 Model Parametreleri Özet Tablosu

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    MODEL PARAMETRELERİ ÖZETİ                           │
├─────────────────────────────────────────────────────────────────────────┤
│ TEMEL İYİLEŞME METRİKLERİ                                              │
│ ────────────────────────                                               │
│ Parkinson UPDRS-III iyileşme: %50.5 (STN-DBS, 6-12 ay)                 │
│ Tremor azalması: %80 (1 yıl)                                           │
│ Diskinezi azalması: %60-80                                             │
│ İlaç dozu azalması: %50-56                                             │
│                                                                         │
│ ZAMAN PARAMETRELERİ                                                    │
│ ──────────────────                                                     │
│ İlk programlama: 2-4 hafta post-op                                     │
│ Programlama seans sayısı: 3-6 (minimum 3)                              │
│ Optimal ayar süresi: 90-180 gün                                        │
│ Programlama seans süresi: 20-45 dakika                                 │
│ IGP ile süre azalması: %57                                             │
│                                                                         │
│ RİSK FAKTÖRLERİ AĞIRLIKLARI                                           │
│ ─────────────────────────                                              │
│ Yaş >70: +30 gün                                                       │
│ Kognitif bozukluk: +45 gün                                             │
│ Düşme öyküsü: +20 gün                                                  │
│ Post-op delirium: +14 gün                                              │
│                                                                         │
│ İYİLEŞTİRİCİ FAKTÖRLER                                                │
│ ─────────────────────                                                  │
│ IGP kullanımı: -25 gün                                                 │
│ Deneyimli merkez: -15 gün                                              │
│ İyi levodopa yanıtı: -20 gün                                           │
│ Genç yaş (<60): -15 gün                                                │
│                                                                         │
│ ML MODEL PERFORMANSI                                                   │
│ ────────────────────                                                   │
│ fMRI+LDA optimal parametre tahmini: %88 doğruluk                       │
│ Autoencoder+MLP sınıflandırma: %96 doğruluk                           │
│ IGP programlama süresi: 19.78 dk (vs 45.22 dk CP)                      │
└─────────────────────────────────────────────────────────────────────────┘
```

### 10.3 Kaynaklar ve Referanslar

**Meta-analizler:**
1. Subthalamic and pallidal deep brain stimulation for Parkinson's disease—meta-analysis of outcomes. npj Parkinson's Disease (2021)
2. Deep Brain Stimulation: A Systematic Review (Frontiers in Aging Neuroscience, 2023)

**Klinik Çalışmalar:**
3. Image-guided programming deep brain stimulation improves clinical outcomes. npj Parkinson's Disease (2024)
4. Accelerated symptom improvement in Parkinson's disease via remote internet-based optimization. Communications Medicine (2025)
5. Predicting optimal DBS parameters using functional MRI and machine learning. Nature Communications (2021)

**Klinik Kılavuzlar:**
6. Physical Therapist Management of Parkinson Disease: APTA Clinical Practice Guideline (2022)
7. European Physiotherapy Guideline for Parkinson's Disease
8. German DBS Guidelines for Parkinson's Disease

**Uzun Vadeli Sonuçlar:**
9. Deep Brain Stimulation Still Effective After 15 Years. Neurology (2021)
10. Deep Brain Stimulation in Parkinson's Disease: Still Effective After More Than 8 Years. Movement Disorders Clinical Practice (2020)

---

## Ekler

### Ek A: UPDRS-III Alt Skorları

| Alt Skor | Açıklama | Max Puan |
|----------|----------|----------|
| Konuşma | Konuşma bozukluğu | 4 |
| Yüz ifadesi | Hipomimi | 4 |
| Tremor (istirahat) | El, ayak, çene | 20 |
| Aksiyon tremoru | El | 8 |
| Rijidite | Boyun, üst/alt ekstremite | 20 |
| Parmak vuruşu | Bradikinezi | 8 |
| El hareketleri | Açma/kapama | 8 |
| Hızlı el rotasyonu | Pronasyon/supinasyon | 8 |
| Ayak çalma | Bradikinezi | 8 |
| Sandalyeden kalkma | Fonksiyonel | 4 |
| Postür | Duruş bozukluğu | 4 |
| Yürüyüş | Gait analizi | 4 |
| Postural stabilite | Pull test | 4 |
| Vücut bradikinezisi | Genel yavaşlama | 4 |
| **TOPLAM** | | **108** |

### Ek B: Komplikasyon Oranları

| Komplikasyon | Oran | Zaman Aralığı |
|--------------|------|---------------|
| Enfeksiyon | %3-6 | 0-6 ay |
| İntrakranyal kanama (toplam) | %2.3 | İntra/post-op |
| Major ICH | %0.7 | İntra/post-op |
| Cihaz arızası | %5-10 | >1 yıl |
| Elektrot migrasyonu | %1-2 | Değişken |
| IPG cep problemleri | %3-5 | >6 ay |
| Re-operasyon gerekliliği | %15-20 | 5 yıl içinde |

### Ek C: Stimülasyon Parametreleri Referans Tablosu

| Hedef | Frekans (Hz) | Puls Genişliği (μs) | Voltaj (V) |
|-------|--------------|---------------------|------------|
| STN | 130-185 | 60-90 | 2.0-3.5 |
| GPi | 130-185 | 60-120 | 2.5-4.0 |
| VIM | 130-185 | 60-90 | 2.0-3.5 |
| ATN | 145 | 90 | 3.5-5.0 |

---

*Bu döküman, DBS sonrası iyileşme ve optimal süre modelleme projesi için hazırlanmıştır.*
*Son güncelleme: 31 Ocak 2026*
*Görkem Ergüne*