#  Test Planı: Yanvar 2026 Sprint (v5.4.0)

Bu plan Kapital Bank mobil tətbiqinin yanvar ayı buraxılışı üçün nəzərdə tutulan konkret icraatları əhatə edir.

## 1. Test Resursları
* **QA Engineer:** [Fidan Atayeva ]
* **Test Cihazları:**  iPhone 14 (iOS 17)
  * Samsung Galaxy A54 (Android 14)

## 2. Test Cədvəli (Milestones)
| Fəaliyyət | Start | End |
| :--- | :--- | :--- |
| Test Case Yazılması | 21.01.2026 | 22.01.2026 |
| İlk Test İcrası (Execution) | 23.01.2026 | 26.01.2026 |
| Regressiya Testi | 27.01.2026 | 28.01.2026 |

## 3. Giriş və Çıxış Meyarları
* **Entry:** Build-in stabil olması və test mühitinin (Staging) əlçatanlığı.
* **Exit:** Bütün P0/P1 xətaların bağlanması, test ssenarilərinin 100% icrası.

## 4. Test Ssenariləri (High-Level Test Cases)
1. OTP kodun 60 saniyə ərzində çatmasının yoxlanılması.
2. Kartdan-karta 100 AZN köçürmə zamanı komissiyanın düzgün hesablanması.
3. Yanlış PİN daxil edildikdə istifadəçiyə xəbərdarlıq edilməsi.

## 5. Risklər
* **Gecikmə:** SMS serverində yarana biləcək problemlər test müddətini uzada bilər.
* **Həlli:** Test üçün öncədən təyin edilmiş statik OTP kodlardan istifadə.
