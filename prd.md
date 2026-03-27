# 📋 PRD - Ürün Gereksinim Belgesi (VibeRoute)

Bu belge, yapay zeka destekli kariyer rehberlik uygulamasının teknik ve işlevsel gereksinimlerini tanımlar.

---

## 1. Kullanıcı Akışı (User Flow)
Uygulama açıldığında deneyimi tamamen kişiselleştirmek için kategori seçimi yapılır:
* *Giriş Ekranı:* "Lise Öğrencisiyim" | "Üniversite Öğrencisiyim" butonları.
* *Form Ekranı:* Seçilen kategoriye özel dinamik soruların sorulması.
* *Analiz Süreci:* Verilerin Gemini API'ye gönderilmesi ve işlenmesi.
* *Sonuç Ekranı:* AI tarafından oluşturulan karakter analizi ve kariyer rotası.

---

## 2. Dinamik Soru Setleri (Veri Toplama)
00000000000
### *A. Lise Öğrenci Formu (Gelecek Tasarımı)*
1.  *Akademik Alan:* Mevcut veya hedeflenen alan (Sayısal, Sözel, EA, Dil).
2.  *Güçlü Yön Analizi:* Hangi yönünü daha baskın/güçlü buluyorsun? (Analitik düşünme, yaratıcılık, sosyal iletişim vb.)
3.  *İlgi Odakları:* Neler ilgini çeker? Neler kesinlikle ilgini çekmez?
4.  *Tutku & Hobi:* Boş zamanlarında seni en çok ne mutlu eder?
5.  *Heyecan Faktörü:* Seni ne heyecanlandırır? (Yeni bir şey icat etmek, insanlara yardım etmek, yönetmek vb.)

### *B. Üniversite Öğrenci Formu (Kariyer Dönüşümü)*
1.  *Mevcut Uzmanlık:* Okuduğun bölüm/fakülte nedir?
2.  *Güçlü Yön Analizi:* Kendi karakterinde ve becerilerinde en güçlü bulduğun yönün nedir? (Kriz yönetimi, detaycılık, liderlik, teknik çözümleme vb.)
3.  *Çalışma Tercihi:* Hareketli bir "Saha" ortamı mı, odaklanmış bir "Masa Başı" düzeni mi?
4.  *Sosyal İhtiyaç:* İnsanlarla sürekli etkileşim mi, yoksa bireysel/teknik çalışma mı?
5.  *Negatif Filtre:* Neleri yapmaktan kesinlikle hoşlanmazsın? (Rutin işler, aşırı stres, sürekli raporlama vb.)
6.  *Motivasyon & Heyecan:* Temel motivasyon kaynağın nedir? Seni ne heyecanlandırır?
7.  *Sektörel Hedef:* Özel sektörün dinamizmi mi, devlet kurumunun güvencesi mi?

---

## 3. Yapay Zeka Çıktı Mimarisi (Gemini AI Output)
Gemini, toplanan verileri şu yapılandırılmış şablona göre sunar:

| Başlık | İçerik Açıklaması |
| :--- | :--- |
| *Karakter Analizi* | Kullanıcının girdiği verilere dayanarak oluşturulan derinlemesine "Karakter Portresi". |
| *Önerilen 3 Rota* | Karakter, güç alanları ve uzmanlıkla %100 uyumlu 3 modern meslek/pozisyon önerisi. |
| *"Uzak Dur" Uyarısı* | Kullanıcının "sevmedikleri" ve "heyecan duymadıkları" listesine göre kaçınması gereken alanlar. |
| *Gelişim Yol Haritası* | Önerilen rotalar için geliştirilmesi gereken kritik beceriler (Soft & Hard Skills). |
| *Samimi Mentor Notu* | Kullanıcıya özel, samimi, teşvik edici ve vizyon katan kapanış mesajı. |

---

## 4. Teknik Gereksinimler
* *Model:* Google Gemini Pro (Text-to-Text Analysis).
* *Veri Yönetimi:* Kullanıcı form verilerinin JSON formatında AI'ya iletilmesi.
*
