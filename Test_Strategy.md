# Test Strategiyası: Kapital Bank Mobil Tətbiqi

Bu sənəd "Birbank" layihəsi üzrə keyfiyyət təminatının ümumi prinsiplərini və metodoloji yanaşmasını müəyyən edir.

## 1. Test Yanaşması (Testing Approach)
Layihədə **Risk-Based Testing** (Riskə əsaslanan test) yanaşması tətbiq olunur. Kritik maliyyə funksiyaları (köçürmələr, təhlükəsizlik) ən yüksək prioritetlə test edilir.

## 2. Testin Əhatə Dairəsi (Scope)
* **In-Scope:** Giriş modulu, P2P köçürmələr, Kommunal ödənişlər, QR-pay.
* **Out-of-Scope:** Backend verilənlər bazasının birbaşa modifikasiyası, ATM aparat təminatı.

## 3. Test Səviyyələri və Növləri
* **System Testing:** Sistemin bütöv şəkildə funksional yoxlanışı.
* **API Testing:** Rest-API servislərinin validasiyası.
* **Security Testing:** Şəxsi məlumatların və tranzaksiyaların təhlükəsizliyi.
* **Compatibility Testing:** Müxtəlif cihaz və OS versiyalarında uyğunluq.

## 4. İstifadə Olunacaq Alətlər
* **Postman:** API testləri üçün.
* **Jira:** Defektlərin izlənilməsi (Bug Tracking) üçün.
* **Charles Proxy:** Şəbəkə trafikinin monitorinqi üçün.

## 5. Defekt İdarəetməsi (Defect Management)
Baqlar Jira-da qeyd olunur və aşağıdakı prioritetlərə bölünür:
* **P0 (Blocker):** Tətbiq açılmır və ya əsas maliyyə funksiyası işləmir.
* **P1 (Critical):** Vacib funksiya xətalıdır, alternativ yol yoxdur.
* **P2 (Major):** Funksiya işləyir, amma ciddi vizual və ya məntiqi qüsur var.
* **P3 (Minor):** Kiçik vizual xətalar.
