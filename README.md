# YKS-Veritaban-Uygulamas-
OOP Lab proje ödevi olarak yaptığımız öğretmen öğrenci için yks veritabanı uygulaması
# 🎓 NetSkor - YKS Takip Sistemi

**NetSkor**, Yükseköğretim Kurumları Sınavı (YKS) kapsamında öğrencilerin deneme sınavı ve pratik çalışmalarını kayıt altına alıp takip edebilmeleri için geliştirilen bir Java tabanlı veritabanı yönetim sistemidir.  
Proje Swing arayüzü ile desteklenmiş olup öğretmen ve öğrenci girişleri ayrı ayrı ele alınmıştır.

---

## 📁 Proje Yapısı

```
src/
├── database/         # Veritabanı bağlantı sınıfı (DatabaseConnector)
├── gui/              # Swing tabanlı grafik arayüz (MainFrame, EntryForms, Menüler)
├── main/             # Uygulamanın başlangıç noktası (Main.java)
├── manager/          # Kayıt yönetimi sınıfları (TYT/AYTRecordManager, PersonManager)
├── models/           # Öğrenci, öğretmen ve kişi sınıfları (Ogrenci, Ogretmen, Person)
├── records/          # TYT/AYT sınav ve pratik kayıtları
├── util/             # Yardımcı sınıflar (PasswordUtil, QuestionStats)
```

---

## 🚀 Başlangıç

### Gerekli Kurulumlar

- Java JDK 8+
- MySQL Server
- Eclipse / IntelliJ IDEA (Tavsiye edilen geliştirme ortamı)

### Projeyi Çalıştırmak için

1. Veritabanını oluşturun ve tabloları içeren SQL dosyasını çalıştırın.
2. `DatabaseConnector.java` dosyasındaki bağlantı bilgilerini kendi sisteminize göre güncelleyin:
   ```java
   String url = "jdbc:mysql://localhost:3306/yks_tyt_ayt";
   String user = "root";
   String password = "şifre";
   ```
3. `Main.java` dosyasını çalıştırarak uygulamayı başlatın.

---

## 🧑‍🏫 Özellikler

- Öğrenci kayıt ve giriş sistemi
- Öğretmen kayıt ve giriş sistemi
- TYT ve AYT için:
  - Sınav sonuçlarını ekleme
  - Pratik sonuçlarını ekleme
  - Net hesaplama
  - Sonuç görüntüleme
- Swing arayüz desteği
- MySQL veritabanı bağlantısı

---

## 🗃️ Veritabanı Yapısı

- `student`, `teacher`, `person` tabloları
- `TYTExamRecord`, `TYTPracticeRecord`, `AYTExamRecord`, `AYTPracticeRecord` tabloları
- `studentNo`, `ogretmenID`, `practiceId`, `examId` gibi birincil anahtarlar
- Yabancı anahtarlarla ilişkilendirilmiş kayıtlar

---

## 🛠️ Kullanılan Teknolojiler

- Java
- Swing
- MySQL
- JDBC

---

## 🧾 UML Diyagramları

Proje içerisinde her `package` için ayrı UML diyagramları hazırlanmıştır.  
Ayrıca tüm sistemi kapsayan birleşik bir UML sınıf diyagramı da mevcuttur (`uml_diagram.puml`).

---

## 👥 Katkıda Bulunanlar

- Kaan Ünal
- Eray Akpınar
- Mehmet Emin Arık

---

## 📜 Lisans

Bu proje MIT Lisansı altında lisanslanmıştır.
