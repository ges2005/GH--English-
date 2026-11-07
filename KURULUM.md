# Kurulum ve Kullanım Rehberi

> Program özel bir uygulama olmadan, **doğrudan Claude üzerinde** (claude.ai ve Claude mobil uygulaması) yürür.
> Dört **Claude Projesi** dört kişiyi temsil eder. Projeler arasındaki köprü iki ortak dosya ve oturum raporlarıdır.

---

## Genel bakış

```
                ┌───────────────────────────────────┐
                │  ortak/ogrenci-dosyasi.md         │  ← her pazar koç günceller,
                │  ortak/program-plani.md (sabit)   │    siz dört projeye yüklersiniz
                └───────────────┬───────────────────┘
       ┌───────────────┬────────┴───────┬───────────────────┐
       ▼               ▼                ▼                   ▼
  Dan Carter      Elif Hoca        Murat Bey          Sınav Görevlisi
  (native)        (Türk öğretmen)  (koç)              (aylık)
  speaking,       gramer, kelime,  günlük LOG,        seviye tespiti,
  B1+ beceriler   A1-A2 beceriler  haftalık/aylık     aylık/ara/bitiş
       │               │           değerlendirme      sınavı
       └── SESSION REPORT ──► Murat Bey'in "Hafta NN" sohbeti ◄── ASSESSMENT REPORT
```

| Proje | Talimat dosyası | Bilgi kaynağına yüklenecek dosyalar |
|---|---|---|
| **Dan Carter – Native Teacher** | `projeler/1-dan-carter-native-teacher/talimat.md` | `persona-karti.md`, `program-plani.md`, `ogrenci-dosyasi.md` |
| **Elif Hoca – Türk Öğretmen** | `projeler/2-elif-hoca-turk-ogretmen/talimat.md` | `hata-haritasi.md`, `program-plani.md`, `ogrenci-dosyasi.md`, `kelime-defteri.md` |
| **Murat Bey – Program Koçu** | `projeler/3-murat-bey-program-kocu/talimat.md` | `program-plani.md`, `ogrenci-dosyasi.md` |
| **Sınav Görevlisi (Examiner)** | `projeler/4-sinav-gorevlisi/talimat.md` | `program-plani.md`, `ogrenci-dosyasi.md` |

---

## 0. Gerekenler

- **Claude hesabı.** Programda günde 2-3 saat yoğun kullanım var. Ücretsiz planın limitleri büyük ihtimalle yetmez; ücretli bir plan (Pro veya üstü) önerilir.
- **Telefonda Claude uygulaması:** sesli mod (speaking ve listening) için.
- **Bilgisayar veya tablet:** yazma ve dosya yükleme için daha rahattır.
- **Bu repodaki dosyalar:** GitHub'da **Code → Download ZIP** ile indirebilirsiniz.
- **Takvim/alarm:** Claude size kendiliğinden yazmaz; günlük çalışma saatlerini ve pazar koç görüşmesini takvime siz koyarsınız.
- **Birden fazla kişi öğreniyorsanız:** Her kişinin kendi hesabı (veya en azından kendi dört projesi ve kendi öğrenci dosyası) olmalı.

---

## 1. Projeleri oluşturun (≈20 dk)

Her proje için:
1. claude.ai → **Projects** → **Create project**.
2. Adı yukarıdaki tablodan verin.
3. **Instructions** (proje talimatı) kutusuna, ilgili `talimat.md` dosyasındaki **kod bloğunun içini** yapıştırın. GitHub'da kod bloğunun sağ üstündeki kopyala düğmesini kullanabilirsiniz.
4. **Knowledge** (bilgi kaynağı) bölümüne tablodaki dosyaları yükleyin.

> İsimleri, yaşları ya da memleketleri değiştirmek isterseniz söylemeniz yeterli; tüm dosyalarda tutarlı biçimde güncellenmesi gerekir.

**Ayarlar:** Claude'un ayarlarında hafıza (memory) veya geçmiş sohbetleri arama özellikleri varsa açabilirsiniz. Öğretmenin aynı proje içindeki önceki derslerinizi hatırlamasına yardım eder. Yine de asıl kaynak dosyalar ve raporlardır.

---

## 2. Kurulumu test edin (≈10 dk)

| Test | Beklenen |
|---|---|
| Dan projesinde yeni sohbet açın ve Türkçe *"Merhaba, nasılsın?"* yazın | İngilizce cevap verir, Türkçe konuşmaz, sizi İngilizceye yönlendirir. |
| Dan projesinde metinle açın (`SESSION: SPEAKING | Week 01 | Theme: Me & my life`), sonra **aynı sohbette** sesli moda geçin | Sesli modda da Dan gibi, kısa cümlelerle konuşur. |
| Sesli mod ayarlarında sesleri dinleyin | Size en çok Amerikan İngilizcesi gibi geleni seçin. Sesli mod hazır seslerle çalışır; aksan talimatla değiştirilemez. |
| Elif projesinde `SESSION: GRAMMAR | Week 01` yazın | Türkçe-İngilizce karışık ve yönlendirici bir ders açılır. |
| Koç projesinde *"Merhaba"* yazın | Kendini tanıtır, KURULUM'a yönlendirir. |

---

## 3. Gün 0: Seviye tespiti ve açılış (≈2 saat)

1. **EF SET** (önerilen, ücretsiz, ~50 dk, okuma ve dinleme): Claude ses dinletemediği için dinleme seviyenizi en iyi dış ölçüt verir.
2. **Sınav Görevlisi** → yeni sohbet → `SESSION: PLACEMENT`. Test bitince ASSESSMENT REPORT'u kopyalayın.
3. **2 dakikalık konuşma kaydı** (telefonun ses kaydedicisiyle): *"Introduce yourself. Talk about your daily life, why you are learning English, and your plans for the future."* Kaydı saklayın; Hafta 13 ve 26'da aynı soruyla karşılaştıracaksınız.
4. **Murat Bey** → yeni sohbet (adı: *Kurulum*) → `KURULUM` yazın. Placement raporunu ve EF SET sonucunu yapıştırın, görüşmeyi tamamlayın. Koç doldurulmuş `ogrenci-dosyasi.md`'yi verir.
5. Bu dosyayı **dört projede de** değiştirin: eski boş dosyayı silin, yenisini yükleyin.
6. Murat Bey'de **"Hafta 01"** (veya koçun seçtiği başlangıç haftası), Elif Hoca'da **"Kelime – Hafta 01"** sohbetlerini açın.
7. Takvime günlük çalışma bloklarını ve **pazar koç görüşmesini** ekleyin.

---

## 4. Günlük akış

| # | Nerede | Ne yaparsınız |
|---|---|---|
| 1 | Elif → **"Kelime – Hafta NN"** sohbeti (haftalık, aynı sohbet) | `SESSION: VOCAB | Week NN | Day N` → tekrar, yeni kelimeler, mini günlük (25-35 dk) |
| 2 | Günün oturumları (bkz. `program-plani.md` → Haftalık ritim) | Her oturum için ilgili projede **yeni sohbet** → açılış satırı → oturum → `REPORT` |
| 3 | Murat Bey → **"Hafta NN"** sohbeti | Her raporu kopyalayıp yapıştırın; günün sonunda **LOG** satırını yazın. Koç 3-4 satırla cevap verir. |

**Mesaj şablonları:**

Oturum açılışı:
```
SESSION: SPEAKING | Week 07 | Theme: Travel | Note: role-play hotel check-in, 30 min
```

Oturum kapanışı:
```
REPORT
```

Günlük LOG (dakika cinsinden):
```
LOG 2026-11-09 | Vocab 30 (18 new, review 80%) | Reading 35 | Listening 0 | Writing 0 | Speaking 30 | Grammar 40 | Extra 20 (series) | Energy 4/5 | Note: ...
```

Raporun son satırını (*Student: energy _/5 · hardest part: ___*) koça yapıştırmadan önce siz doldurun.

---

## 5. Haftalık akış (pazar, ≈30 dk)

1. **Elif → "Kelime – Hafta NN":** Hafta sonu kelime testi → `HAFTAYI KAPAT` → yeni `kelime-defteri.md` → Elif projesinde dosyayı değiştirin.
2. **Murat Bey → "Hafta NN":** `HAFTALIK DEĞERLENDİRME` → görüşme → yeni `ogrenci-dosyasi.md` → **dört projede** değiştirin.
3. Yeni hafta için yeni sohbetleri açın: Murat Bey'de **"Hafta NN+1"**, Elif'te **"Kelime – Hafta NN+1"**.

---

## 6. Aylık akış (Hafta 4, 8, 13, 17, 21, 26)

1. **Sınav Görevlisi:** `SESSION: MONTHLY | Week NN` (Hafta 13'te `MIDTERM`, Hafta 26'da `FINAL`) → ASSESSMENT REPORT.
2. **Elif → kelime sohbeti:** `AY SONU TESTİ` → arşiv listelerini kendi `kelime-arsivi.md` dosyanıza ekleyin (projeye yüklemeyin) ve küçültülmüş `kelime-defteri.md`'yi projeye yükleyin.
3. **Hafta 13 ve 26:** EF SET'i tekrarlayın; aynı soruyla 2 dakikalık konuşma kaydı yapıp Gün 0 kaydıyla karşılaştırın.
4. **Murat Bey:** `AYLIK DEĞERLENDİRME` + sınav raporu (ve varsa EF SET) → faz, çalışma seviyesi, Türkçe oranı kararı → yeni `ogrenci-dosyasi.md` → dört projeye yükleyin.

---

## 7. Sohbet düzeni

| Sohbet türü | Örnek ad | Ömrü |
|---|---|---|
| Oturum | `2026-11-09 Speaking – Hotel` | Tek oturum |
| Kelime | `Kelime – Hafta 07` | Bir hafta |
| Koç | `Hafta 07` | Bir hafta |
| Sınav | `Monthly – Week 08` | Tek sınav |

Uzun sohbetlerde talimatlar zayıflar ve kullanım limitiniz daha hızlı dolar. Bu yüzden oturum sohbetlerini uzatmayın.

---

## 8. Sesli mod: speaking, listening ve telaffuz

- **Persona garantisi:** Sohbeti önce metinle açın (`SESSION: ...`), sonra aynı sohbette sesli moda geçin. Böylece persona ve oturum bağlamı kesin yüklenmiş olur.
- **Rapor:** Sesli konuşma bitince metne dönüp `REPORT` yazın. Uzun bir raporun sesli okunması gereksizdir.
- **Telaffuz kontrolü:** Claude sesinizi değil, sesinizin yazıya çevrilmiş halini görür. Ekrandaki transkripte bakın: Söylediğiniz kelime yanlış yazıldıysa o kelimede anlaşılırlık sorunu var demektir.
- **Telaffuz pratiği:** Kelimenin doğru sesini sözlükte (ör. Cambridge Dictionary, US sesi) veya YouGlish'te dinleyin, kendinizi kaydedip karşılaştırın.
- **Sesli modla listening:** *"Tell me a short story at my level, then ask me three questions."* Claude'un sesiyle etkileşimli dinleme pratiği yaparsınız.

---

## 9. Claude dışında kullanılacak minimum kaynaklar

Claude'un yapamadığı birkaç şey var. Bunlar uygulama geliştirmek değil, sadece içerik kaynakları:

| İhtiyaç | Neden | Kaynak örnekleri |
|---|---|---|
| Gerçek Amerikan aksanı ve doğal hızda konuşma | Claude dış ses dinletemez | VOA Learning English (yavaş, dökümlü), ders amaçlı podcastler, TED (döküm), Amerikan diziler İngilizce altyazıyla, B2+'da NPR podcastleri |
| Kapsamlı okuma | Keyifli ve bol okuma | Kademeli okuma kitapları (Oxford Bookworms, Penguin Readers vb.), sonra otantik metinler |
| Dış seviye ölçümü | Claude'un tahmini doğrulanmalı | EF SET (ücretsiz) |
| Telaffuz kalibrasyonu (opsiyonel) | Claude telaffuzu duyamaz | Hafta 13 ve 26'da gerçek bir öğretmen veya konuşma partneriyle 30 dk |

**Dökümü olan sesi** dinledikten sonra dökümü öğretmene yapıştırırsınız; analiz Claude'da yapılır (bkz. `program-plani.md` → LISTENING).

---

## 10. Sorun giderme

| Sorun | Çözüm |
|---|---|
| Dan Türkçe konuştu veya persona bozuldu | Yeni sohbet açın; uzun sohbetlerde kurallar zayıflar. Tekrarlıyorsa talimat sıkılaştırılabilir. |
| Dan'ın İngilizcesi çok zor | *"Please simplify. I'm A2."* yazın; öğrenci dosyasındaki ÇALIŞMA SEVİYESİ'ni kontrol edin. |
| Elif çok fazla Türkçe (veya çok az) konuşuyor | Öğrenci dosyasındaki TÜRKÇE ORANI'nı kontrol edin; koça söyleyin, haftalık güncellemede ayarlansın. |
| Sesli modda persona yok | Sohbeti metinle açıp sonra sesli moda geçin. |
| Kullanım limitine takılıyorum | Oturum sohbetlerini kısa tutun; haftalık sohbetlere sadece rapor ve LOG yapıştırın; dinleme ve okumanın bir kısmını dış kaynakla yapın; gerekirse planınızı yükseltin. |
| Kelime tekrarı çok uzun sürüyor | Günlük yeni kelimeyi 10-15'e düşürün. Elif'ten tekrar kelimelerini etkileşimli kart (artifact) olarak hazırlamasını isteyin. |
| Dosyayı güncellemeyi unuttum | Koçun son sohbetinde en son verdiği dosyayı tekrar isteyin ve yükleyin. |
| Bir gün çalışamadım | Minimum gün yapın (20 dk). İki gün üst üste kaçırmayın. Koça LOG'da durumu yazın. |
| Hedefin gerisindeyim | Aylık değerlendirmede koçla hedefi veya günlük süreyi birlikte revize edin. Sessizce bırakmak en kötü seçenektir. |

---

## 11. (Opsiyonel) Dosya güncellemelerini hızlandırmak

Haftalık dosya yükleme manuel yapılır ve ~3-5 dakika sürer. Hesabınızda **Google Drive** bağlantısı varsa `ogrenci-dosyasi.md`'yi Google Docs'ta tutup projelere Drive üzerinden eklemeyi deneyebilirsiniz. Projelerin dosyanın güncel sürümünü kullanıp kullanmadığını kendi hesabınızda test edin. Çalışırsa haftalık yükleme adımı kısalır; çalışmazsa manuel yöntemle devam edin.
