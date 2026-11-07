# İngilizce Öğrenme Programı: Kurgu Değerlendirme Raporu

> Kapsam: Claude üzerinde kurulacak 3 ajanlı (Amerikalı öğretmen, Türk öğretmen, program koordinatörü) 6 aylık İngilizce programının değerlendirmesi, riskleri ve iyileştirme önerileri.
> Tarih: Kasım 2026

---

## 0. Kısa hüküm

**Kurgu sağlam bir temele oturuyor.** Rol ayrımı, iyi bir dil okulunun yapısını taklit ediyor: anadili İngilizce olan öğretmen + öğrencinin dilini bilen öğretmen + akademik danışman. Türk hocanın İngilizce oranını seviyeye göre artırması da doğru bir yaklaşım; araştırmalar da ana dilin (Türkçenin) ölçülü kullanımını destekliyor.

Ancak kurgunun **beş önemli açığı** var. Bunlar giderilmezse program 2-3. ayda tıkanır:

1. **Hedef/süre gerçekçiliği:** Sıfırdan 6 ayda C1, günde 4-5 saat gerektirir. Hedef başlangıç seviyesine ve günlük süreye göre yeniden tanımlanmalı.
2. **Ajanlar arasında ortak hafıza yok:** Üç ajan birbirinin ne yaptığını bilmez. Hepsinin okuyup beslediği **tek bir “öğrenci dosyası”** şart.
3. **Claude’un ses ve telaffuz sınırları:** Claude’a “Amerikan aksanı” persona talimatıyla verilemez ve sesli modda sizin telaffuzunuzu gerçekten “duyamaz”, çünkü konuşmanız önce metne çevrilir. Speaking ve listening için dış kaynak ve araç gerekir.
4. **“Kelime ezberi” yaklaşımı:** Liste ezberi verimsizdir. Aralıklı tekrar (SRS, ör. Anki) ve bağlam içinde öğrenme şart. “Kaç kelime ezberledik” yerine “kaç kelime kalıcı oldu” ölçülmeli.
5. **Ölçme-değerlendirme eksik:** Seviye tespiti, ara sınav, bitiş sınavı ve dış (Claude dışı) bir ölçüt yok. Yapay zekâ öğretmenler not vermede cömert olma eğilimindedir.

Aşağıda her başlığı ayrıntılandırıp somut çözümler, haftalık program, 6 aylık faz planı ve ajan talimatı taslakları sunuyorum.

---

## 1. Kurgunun güçlü yanları

| Unsur | Neden iyi |
|---|---|
| **Anadili İngilizce öğretmen, Türkçe bilmiyor** | Sizi İngilizce düşünmeye ve anlamadığınızda “İngilizceyle çözmeye” zorlar. Gerçek hayattaki iletişim baskısının en yakın simülasyonu budur. |
| **Türk öğretmen, İngilizce oranını kademeli artırıyor** | Krashen’in “anlaşılabilir girdi” (i+1) fikrine uyuyor: biraz zorlayan ama anlaşılır dil. Başta Türkçe güven verir, sonra İngilizce yükü artar. |
| **Türk öğretmenin karşılaştırmalı bakışı** | Bir Türk’ün nerede hata yapacağını (article’lar, he/she, present perfect, kelime sırası vb.) en iyi Türkçeyi bilen öğretmen öngörür. Bu çok değerli bir rol. |
| **Ayrı bir koç/koordinatör** | Dil öğrenimindeki başarısızlığın 1 numaralı sebebi yöntem değil **devamlılıktır**. Takip ve hesap sorma rolü bunu doğrudan hedefliyor. |
| **4 beceri + kelime + speaking** | Sadece gramer/kelime değil, bütün becerileri kapsıyor. |
| **Sizin sorunlarınızı ve isteklerinizi dinleyen bir yapı** | Esnek ve kişiselleştirilebilir. |

---

## 2. Kritik riskler ve gerçekçilik kontrolü

### 2.1 Altı ayda B2-C1 hedefi: saat hesabı

Cambridge’in yaygın kullanılan tahminine göre bir seviyeye ulaşmak için gereken **toplam (sıfırdan, kümülatif) rehberli öğrenme saatleri** kabaca şöyle:

| Seviye | Yaklaşık toplam saat |
|---|---|
| A2 | 180-200 |
| B1 | 350-400 |
| B2 | 500-600 |
| C1 | 700-800 |

6 ay ≈ 26 hafta. Haftada 6 gün çalışırsanız ≈ 156 çalışma günü eder. Buna göre **günlük gereken süre**:

| Başlangıç → Hedef | Gereken ek saat (yaklaşık) | Günlük süre (haftada 6 gün) |
|---|---|---|
| Sıfır (A0) → B2 | ~550 | **~3,5 saat** |
| Sıfır (A0) → C1 | ~750 | **~4,8 saat** |
| A2 → B2 | ~360 | **~2,3 saat** |
| A2 → C1 | ~560 | **~3,6 saat** |
| B1 → B2 | ~175 | **~1,1 saat** |
| B1 → C1 | ~375 | **~2,4 saat** |

**Notlar:**
- Bunlar kaba tahminlerdir. Birebir öğretim, sınıf ortamından daha verimli olabilir. Öte yandan Türkçe ile İngilizce yapısal olarak uzak diller (kelime sırası, article yok, ek yapısı farklı), bu da süreyi uzatabilir.
- Algılama becerileri (reading, listening) genelde üretim becerilerinden (speaking, writing) **önce** ilerler. 6. ayın sonunda “okuma B2, konuşma B1+” gibi bir profil çok normaldir.

**Öneri:** Hedefi tek bir harf olarak değil, **beceri bazında** tanımlayın:

> **6. ay sonu gerçekçi hedef (A1-A2 başlangıç, günde ~3 saat):** Reading/Listening **B2**, Writing **B1+/B2**, Speaking **B1+/B2**. **C1** hedefini 9-12. aylara koyun.
> Başlangıç seviyeniz B1 veya üstündeyse C1 hedefi 6 ayda konuşulabilir.

Bunun için **ilk iş seviye tespiti** olmalı (bkz. §8).

### 2.2 Claude’un teknik sınırları

| Kurgudaki varsayım | Gerçek durum | Çözüm |
|---|---|---|
| “Amerikan aksanıyla konuşuyor” | Metin sohbette aksan yoktur. Sesli modda ise hazır seslerden biri seçilir; persona talimatıyla aksan belirlenemez ve kişiye özel ses yaratılamaz. | Personanın “Amerikalılığı” metinde **Amerikan İngilizcesi** demektir: yazım (color), kelime (apartment, fall), deyim, kültür ve telaffuz rehberliği. Gerçek Amerikan aksanını **otantik ses kaynaklarından** dinleyin (§5.3). |
| “Speaking’de telaffuzumu düzeltir” | Sesli modda konuşmanız önce metne çevrilir ve model metni görür. Konuşma tanıma sistemi yanlış telaffuzu çoğu zaman “doğru kelimeye” düzelttiği için öğretmen telaffuz hatanızı **göremez**. | (1) Telaffuza özel uygulamalar (ör. telaffuz puanlayan uygulamalar), (2) kendinizi kaydedip sözlük ve YouGlish sesleriyle karşılaştırma, (3) shadowing, (4) 2-4 haftada bir 30 dakikalık **insan öğretmen** seansı (italki, Preply, Cambly vb.) ile kalibrasyon. **Pratik ipucu:** Sesli modda ekranda çıkan transkripte bakın. Söylediğiniz kelime yanlış yazıldıysa o kelimede anlaşılırlık sorunu var demektir. |
| “Ajanlar birbirinden haberdar” | Her proje veya sohbet ayrıdır. Claude’un hafıza özellikleri hesaba göre değişse de yapılandırılmış ilerleme verisi (saatler, kelime sayıları, hata listesi) için bunlara güvenilmez. | **Tek bir öğrenci dosyası** ve her oturum sonunda standart bir **oturum raporu** (§3.2, §3.3). |
| “Koç bizi takip eder, yönlendirir” | Claude kendiliğinden size yazmaz ve hatırlatma yapmaz. | Takvim ve telefon hatırlatıcıları kurun. Koç, siz yazdığınızda logu okuyarak değerlendirir. |
| “Öğretmen seviyemizi değerlendirir” | Dil modelleri cesaretlendirici olmaya, yani **not şişirmeye** eğilimlidir. | Rubrik (değerlendirme ölçeği) zorunlu olsun, “dürüst ol” talimatı verilsin, ayrı bir “sınav görevlisi” rolü olsun ve **Claude dışı testler** yapılsın (§8). |
| “Türkçe hiç bilmiyor” | Model Türkçeyi bilir. Bu bilgi değil, **davranış** kuralıdır. Uzun sohbetlerde ve Türkçe yazdığınızda kayabilir. | Talimata net kural yazın (Türkçe yazılırsa nasıl tepki verileceği) ve her oturumu **yeni sohbette** başlatın. |
| Seviyeye uygun dil | Modeller varsayılan olarak fazla zengin İngilizce kullanır. A1-A2’de bu boğucu olur. | Talimata seviyeye göre dil sınırı yazın (kısa cümle, sık kelimeler, mesaj başına en fazla 2-3 yeni kelime). |
| Uzun sohbetler | Çok uzun sohbetlerde persona ve kurallar zayıflar. | Her oturum için yeni sohbet açın. Öğrenci dosyası ve oturum raporlarıyla süreklilik sağlayın. |

### 2.3 Ajanlar arası bilgi akışı

Mevcut kurguda en büyük yapısal eksik bu. Örnek: Amerikalı öğretmen speaking’de her seferinde article hatası yaptığınızı görüyor. Bu bilgi Türk hocaya ulaşmazsa Türk hoca bu konuyu çalıştırmaz. Koça ulaşmazsa koç “article’lar 3 haftadır düzelmiyor” diyemez.

**Çözüm:** “Hub and spoke” (merkez ve kollar) yapısı. Merkezde **öğrenci dosyası** durur. Her ajan oturum başında bu dosyayı okur, oturum sonunda rapor üretir ve rapor dosyaya eklenir. Koç, haftalık olarak bütün dosyayı analiz eder.

```
             ┌──────────────────────────┐
             │     ÖĞRENCİ DOSYASI      │
             │ profil · plan · log ·    │
             │ kelimeler · hata defteri │
             │ oturum raporları · testler│
             └──────────┬───────────────┘
        okur/rapor ▲    │    ▲ okur/rapor
     ┌─────────────┘    │    └─────────────┐
 Amerikalı öğretmen  Türk öğretmen   Koç/Koordinatör
                                     (haftalık analiz,
                                      plan güncelleme)
```

### 2.4 “Kelime ezberi” oturumu

- Liste ezberi kısa vadede işe yarar gibi görünür ama unutma eğrisi yüzünden kelimelerin büyük kısmı haftalar içinde kaybolur.
- **Aralıklı tekrar (SRS):** Kelimeyi tam unutmak üzereyken tekrar eder. Bu iş için Anki en yaygın ve ücretsiz araçtır (iOS sürümü ücretlidir). Claude tekrarları zamanlayamaz, o yüzden **tekrarı Anki’ye, öğretmeyi Claude’a** bırakın.
- “Kaç kelime ezberledik” yanıltıcı bir metriktir. Doğru metrikler: **olgunlaşmış kart sayısı** (21+ gün aralığa ulaşmış kartlar), **tekrar doğruluk oranı** (%85-90 iyidir) ve **aktif kullanılan kelime** (yazı ve konuşmada kullanılanlar).

Ayrıntı §5.1’de.

### 2.5 Becerilerin kopuk oturumlarda çalışılması

Ayrı oturumlar fikri iyi, ama her oturum farklı bir konudaysa öğrenme dağılır. **Haftalık tema** ile bütünleştirin: Pazartesi okuduğunuz metindeki kelimeler Anki’ye girsin, çarşamba aynı temada yazın, perşembe aynı temada Amerikalı öğretmenle konuşun. Bir kelimeyi farklı becerilerde 5-7 kez görmek kalıcılığı büyük ölçüde artırır.

### 2.6 Ölçme-değerlendirme eksikliği

Başlangıç seviyesi, ara ölçüm ve bitiş ölçümü yoksa “B2’ye geldik mi” sorusu cevapsız kalır. Ayrıca koçun yönlendirmesi veriye değil hisse dayanır. Bkz. §8.

---

## 3. Önerilen geliştirilmiş mimari

### 3.1 Roller ve seviye bazlı sorumluluk tablosu

**Öneri:** Reading, writing, listening ve kelime oturumları **ayrı ajan olmasın**. Bunlar, öğretmenlerin yürüttüğü **oturum türleri** olsun. Böylece persona sayısı az kalır, süreklilik ve motivasyon artar.

| İş | A1-A2 | B1 | B2+ |
|---|---|---|---|
| **Gramer (açık anlatım)** | Türk hoca (Türkçe ağırlıklı) | Türk hoca (İngilizce ağırlıklı) | Türk hoca (İngilizce, zor konular) + Amerikalı (kullanım ve doğallık) |
| **Kelime tanıtımı** | Türk hoca (Türkçe karşılık serbest) | Türk hoca + Amerikalı (İngilizce tanım) | Amerikalı (İngilizce tanım, eş anlamlılar, nüans) |
| **Reading (yoğun)** | Türk hoca | Amerikalı | Amerikalı |
| **Listening (analiz)** | Türk hoca | Amerikalı | Amerikalı |
| **Writing geri bildirimi** | Türk hoca (hata açıklaması) | Türk hoca (doğruluk) + Amerikalı (doğallık) | Amerikalı (doğallık, üslup) + Türk hoca (inatçı hatalar) |
| **Speaking** | Amerikalı (kısa, kontrollü, 10-20 dk) + Türk hoca (hazırlık) | Amerikalı (30-45 dk) | Amerikalı (45-60 dk, tartışma, sunum) |
| **Telaffuz** | Türk hoca (Türklerin tipik sorunları) + Amerikalı | Amerikalı | Amerikalı |
| **Takip, plan, motivasyon** | Koç | Koç | Koç |
| **Seviye ölçümü** | Sınav görevlisi (aylık) | Sınav görevlisi | Sınav görevlisi |

**Türk hocanın B1-B2 sonrası rolü:** “Sadece zor gramer” yerine **“doğruluk koçu ve editör”** olarak, İngilizce konuşarak devam etmesini öneriyorum. Türklerin inatçı hataları (article, preposition, present perfect) C1’de bile sürer ve bunları Türkçeyle karşılaştırarak çözmek en hızlı yoldur.

**Opsiyonel 4. rol, Sınav görevlisi (Examiner):** Ayda bir kullanılır. Sizi tanımayan, övgü vermeyen, CEFR tanımlayıcıları ve rubriklerle değerlendiren tarafsız bir rol. İyi okullarda “öğreten” ile “ölçen” aynı kişi değildir. İsterseniz bu, koçun ayrı bir modu da olabilir.

### 3.2 Öğrenci dosyası (tek doğruluk kaynağı)

Bu repoda (veya Google Drive’da) şöyle bir yapı önerilir:

```
ogrenci-dosyasi/
├── profil.md            # Kim, neden öğreniyor, hedef, ilgi alanları, uygun saatler,
│                        # beceri bazında güncel seviye (A2/B1...)
├── plan.md              # Güncel faz, bu haftanın teması, haftalık hedefler
├── gunluk-log.md        # Tarih | dakika (kelime/R/L/W/S/gramer) | Anki | enerji 1-5 | not
├── hata-defteri.md      # Hata → doğrusu | kural | kategori | kaç kez | ilk/son görülme
├── kelimeler.csv        # kelime | tür | anlam/tanım | örnek cümle | kaynak | tarih
├── oturum-raporlari/    # 2026-11-08-amerikali-speaking.md ...
├── yazilar/             # Writing ödevleri: ilk taslak + düzeltilmiş + yeniden yazım
├── ses-kayitlari.md     # Aylık konuşma kaydı linkleri (ilerlemeyi duymak için)
└── degerlendirmeler.md  # Test sonuçları (EF SET, ara/bitiş sınavı, rubrik puanları)
```

Her ajan projesinin bilgi kaynağına en azından `profil.md`, `plan.md` ve `hata-defteri.md` eklenir ve haftada bir güncellenir.

**Birden fazla kişi öğreniyorsa** (“biz”): Her kişinin kendi dosyası olmalı ve ajan oturum başında kiminle konuştuğunu bilmeli. Ayrıca birbirinizle İngilizce konuşmanız en değerli ek pratiklerden biri olur.

### 3.3 Oturum sonu raporu standardı

Her öğretmen oturumu bu şablonla bitirir. Raporu kopyalayıp `oturum-raporlari/` klasörüne yapıştırırsınız. Koç bunları okur.

```
=== SESSION REPORT ===
Date:
Teacher / Session type:
Duration (min):
Theme / Topic:
New words & phrases (max 15):
Top 3 errors (wrong → right — short rule):
Pronunciation note:
What went well:
Homework:
Teacher's level observation (per skill, with evidence):
Student self-report (energy 1-5, what was hard):
```

Raporu baştan İngilizce tutmak, onu da küçük bir okuma pratiğine çevirir.

---

## 4. Ajanların ayrıntılı tasarımı

### 4.1 Amerikalı öğretmen

**Kurgunuzdaki haliyle iyi; şu eklemelerle güçlenir:**

- **Kimlik ve “persona kartı”:** İsim, memleket (General American aksanın standart sayıldığı Ortabatı iyi bir seçim, ör. Ohio), ailesi, hobileri, öğretmenlik geçmişi. Bunlar doğal sohbet konuları üretir. Modelin her seferinde farklı bir hayat hikâyesi uydurmaması için bu bilgiler sabit bir dosyada durmalı.
- **Seviyeye göre “öğretmen dili” (teacher talk):** A1’de kısa cümleler, en sık kelimeler, yavaş tempo (yazıda kısa mesaj) ve bol örnek. B2’de tamamen doğal dil, deyimler ve phrasal verb’ler.
- **Türkçe kuralı:** Türkçe yazarsanız kibarca İngilizce cevap verir, İngilizce denemenizi ister ve kullanabileceğiniz bir model cümle sunar. Asla çeviri yapmaz.
- **Düzeltme politikası:** Konuşma sırasında araya girmez. Doğrusunu kendi cümlesinde doğal biçimde tekrarlar (recast). Oturum sonunda en önemli 3 hatayı, 3 daha doğal ifadeyi ve 1 telaffuz ipucunu verir. Her hatayı düzeltmek akıcılığı öldürür. Hiç düzeltmemek ise hataları kalıcılaştırır.
- **Konuşma oranı:** Konuşmanın ~%70’i sizde olmalı. Açık uçlu sorular sorar.
- **Oturum türleri:** Serbest sohbet, rol oyunu (restoran, doktor, iş görüşmesi, telefon), resim betimleme (Claude’a fotoğraf yükleyebilirsiniz), hikâye anlatma, 4/3/2 akıcılık tekniği (aynı hikâyeyi 4, 3, sonra 2 dakikada anlatma), tartışma ve münazara (B1+), sunum (B2), okuma ve dinleme tartışması, yazının doğallık kontrolü.
- **Kültür:** Amerikan günlük hayatı, deyimler, small talk kuralları, bayramlar. Dil sadece gramer değildir.
- **Dürüstlük:** Sıcak ve sabırlıdır, ama hatayı övmez ve seviyeyi şişirmez.

**A1’de Türkçe bilmeyen öğretmen sorunu:** Sıfır seviyede bu öğretmenle çalışmak hayal kırıklığı yaratabilir. Çözüm: Türk hoca ilk hafta **“sınıf dili”ni** öğretir: *Could you repeat that? / What does … mean? / How do you say … in English? / Could you speak more slowly? / I don’t understand. / Can you give me an example?* Bu 15-20 kalıpla Amerikalı öğretmenle 1. günden çalışılabilir.

### 4.2 Türk öğretmen

**Dil oranı kuralı (seviyeye göre):**

| Seviye | Türkçe / İngilizce | Uygulama |
|---|---|---|
| A1 | ~%70 / %30 | Açıklamalar Türkçe; selamlaşma, yönergeler, örnekler ve öğrenilmiş kelimeler İngilizce |
| A2 | ~%50 / %50 | Bildiğiniz kelimelerle anlatılabilecek her şey İngilizce; yeni ve soyut kavramlar Türkçe |
| B1 | ~%20 / %80 | Türkçe yalnızca karşılaştırmada ve tıkandığınız yerde |
| B2+ | <%10 / %90+ | Türkçe yalnızca siz isterseniz veya Türkçe karşılaştırma anlamayı belirgin kolaylaştıracaksa |

**“Sandviç” tekniği:** Önce İngilizce anlat, anlaşılmazsa basitleştir, yine olmazsa Türkçe destek ver, sonra tekrar İngilizceye dön.

**Türklerin tipik gramer sorunları (Türk hocanın hazır “hata haritası”):**

| Sorun | Neden (Türkçe etkisi) | Tipik hata |
|---|---|---|
| a/an/the | Türkçede article yok | *I bought car.* / *The life is beautiful.* |
| he/she karışıklığı | Türkçede tek “o” var | *My sister… he is a doctor.* |
| 3. tekil -s | Türkçede fiil çekimi farklı | *She work in a bank.* |
| Sayıdan sonra çoğul | Türkçede “üç kitap” tekil | *three book* |
| Yardımcı fiil (do/does/did) | Türkçede soru eki kullanılır | *Where you live?* / *I not like it.* |
| Boş özne “it/there” | Türkçede özne düşebilir | *Is very nice.* / *Came yesterday.* |
| “var/yok” → there is / have | Doğrudan çeviri | *In my city has a big park.* |
| Kelime sırası (SOV→SVO) | Fiil sonda | *I every day coffee drink.* |
| Present simple vs continuous | “-iyor” ikisini de karşılayabilir | *I am living in Ankara since 2010.* |
| Present perfect vs past simple | Türkçede -di/-miş ayrımı başka bir eksende | *I have seen him yesterday.* |
| Relative clause | Türkçede niteleyici isimden önce gelir | *the yesterday I bought book* |
| Preposition (in/on/at) | Türkçede hal ekleri var | *at Monday, in the bus* |
| Sayılamayan isimler | Türkçede ayrım yok | *informations, advices* |
| Phrasal verb’ler | Türkçede karşılığı yok | B1-B2’nin en büyük kelime engeli |

**Telaffuz (Türklerin tipik sorunları, Amerikan İngilizcesi odaklı):**

- **th** /θ/ /ð/ → t/d veya s/z (*think → tink, this → dis*)
- **w** ile **v** karışıklığı (*very well → wery vell* veya tersi)
- **/æ/ – /ɛ/ – /ʌ/** ayrımı: *cat / bed / cut* (Türkçede bu bölgede tek “e” ve “a” var)
- **Uzun-kısa ünlüler:** *ship/sheep, full/fool*
- **Kelime başı ünsüz kümeleri:** *school → ıskul, street → sıtrit* (araya veya öne ünlü ekleme)
- **Kelime sonu sertleşmesi:** *bag → bak, dog → dok* (Türkçedeki kitab→kitap kuralının etkisi)
- **-ed sonu:** *worked /t/, played /d/, wanted /ɪd/*; Türkler çoğunlukla *work-ed* der
- **Amerikan r’si:** Dil çarpmaz, kelime sonunda da okunur (*car, water*)
- **Flap T:** *water → “wader”, better → “bedder”* (Amerikan’a özgü)
- **Schwa /ə/ ve vurgusuz heceler:** Türkçede her hece net okunur. İngilizce ise vurgu zamanlı bir dildir, vurgusuz heceler yutulur.
- **Bağlantılı konuşma ve kısaltmalar:** *an apple → “anapple”, going to → gonna*. Kendiniz böyle konuşmasanız bile anlamak için şart.
- **Yazıldığı gibi okuma alışkanlığı:** Türkçe fonetik bir dil. Bu alışkanlık en büyük gizli engeldir. Yeni kelimeyi **önce sesiyle** öğrenin.

**Ders akışı önerisi (gramer):** ısınma (önceki konunun 3 sorusu) → keşif (örnek cümlelerden kuralı siz bulun) → açıklama ve Türkçe karşılaştırma → kontrollü alıştırma → serbest üretim (konuyu kullanarak 5 cümle veya kısa paragraf) → hata analizi → oturum raporu. Konu seçiminin bir kısmı müfredattan, bir kısmı da **hata defterinden** (sizin gerçek hatalarınızdan) gelsin.

### 4.3 Koç / Program koordinatörü

**Görev tanımı:** Koç ders vermez. Ölçer, analiz eder, planlar ve motive eder.

**Takip edilecek göstergeler (KPI):**

| Alan | Gösterge | Hedef/eşik örneği |
|---|---|---|
| Devamlılık | Çalışılan gün, seri (streak), haftalık toplam süre (hedef ve gerçek) | Haftada ≥6 gün; “iki gün üst üste kaçırma” kuralı |
| Denge | Becerilere göre süre dağılımı | Hiçbir beceri haftalık sürenin %10’unun altına düşmesin |
| Kelime | Anki: günlük tekrar tamamlandı mı, yeni kart, doğruluk oranı, olgun kart sayısı | Doğruluk %85-90; birikmiş tekrar < 1 günlük miktar |
| Writing | Haftalık kelime sayısı, 100 kelimede hata sayısı | Hata yoğunluğu aydan aya düşmeli |
| Speaking | Haftalık konuşma dakikası, aylık kayıt karşılaştırması | Duraklama ve “ııı” sıklığı azalmalı |
| Girdi | Okunan sayfa/kelime, dinlenen dakika | Haftalık artış |
| Hatalar | Hata defterindeki en sık 5 hata ve trendi | Aynı hata 3 hafta üst üste → özel müdahale |
| Öznel | Enerji, motivasyon, zorlanma (1-5) | 2 hafta üst üste ≤2 → plan hafifletilir |

**Ritim:**
- **Günlük (2 dk):** `gunluk-log.md`’ye bir satır. Koça mesaj atmak gerekmez.
- **Haftalık (15-20 dk, ör. pazar):** Koç logu ve raporları okur. Ardından 3 güçlü yan, 3 gelişim alanı, sonraki haftanın teması ve **en fazla 3 plan değişikliği** önerir.
- **Aylık (30-45 dk):** Sınav görevlisinin sonuçlarıyla birlikte ilerleme raporu ve faz geçişi kararı verilir.

**Koçun dikkat etmesi gerekenler:**
- **“İstek” ile “ihtiyaç” dengesi:** Öğrenciler zorlandıkları beceriden (genelde speaking veya writing) kaçar ve “daha çok kelime çalışayım” der. Koç isteği dinler ama ihtiyacı korur.
- **Kötü gün protokolü (“minimum gün”):** 20 dakika: Anki + 5-10 dakika İngilizce dinleme. Seriyi bozmamak, mükemmel gün yapmaktan daha önemlidir.
- **Dürüstlük:** Hedeften sapma varsa açıkça söyler. Suçlamaz, çözüm önerir.
- **Dil:** Sorunları ve duyguları tam ifade edebilmeniz için meta konuşmalarda Türkçe serbest olsun. B1’den sonra varsayılan dil İngilizce olsun; bu da ek bir konuşma pratiği olur.

---

## 5. Beceri oturumlarının tasarımı

### 5.1 Kelime

- **Ne kadar?** Yaygın tahminlere göre B2 için yaklaşık 3.500-4.000, C1 için 4.000-5.000+ kelime ailesini (en azından tanıyarak) bilmek gerekir.
- **Günlük yeni kelime:** İlk 2 hafta 10-15, sonra **15-25**. Basit bir kural: günlük tekrar sayısı ≈ günlük yeni kart × 10. Yani 20 yeni kart, yerleşik düzende günde ~200 tekrar ve **30-40 dakika** demektir. Bu süreyi plana mutlaka koyun.
- **6 aylık hesap:** ~156 gün × 18 yeni kelime ≈ 2.800 kelime + okuma ve dinlemeden gelen dolaylı öğrenme + mevcut bilginiz. A2 başlangıçla B2 kelime hedefi bu şekilde ulaşılabilir.
- **Hangi kelimeler?** Önce sıklık: **Oxford 3000** (A1-B2 çekirdek), ardından **Oxford 5000** (B2-C1 eklemeleri). Buna ek olarak kendi alanınızın (iş, hobi) kelimeleri ve okuduklarınızdan “madencilik” ile çıkardığınız kelimeler. C1 için akademik kelime listesi (AWL).
- **Kart tasarımı:** Sadece “kelime → anlam” değil, **cümle içinde** (boşluk doldurma), Amerikan telaffuz sesi ve sık kullanıldığı kalıp (collocation) ile. Aktif kullanmak istediğiniz kelimeler için ters kart (Türkçe/tanım → İngilizce).
- **Çift dilliden tek dilliye geçiş:** A2 sonu ve B1 başından itibaren İngilizce tanımlara geçin (Oxford Learner’s Dictionaries, Cambridge Dictionary; ikisi de Amerikan telaffuzu sunar).
- **Claude’un rolü:** Tekrar yaptırmak değil, **öğretmek**: günün kelimelerini bağlam içinde sunmak, kelime ailesi (decide, decision, decisive), sık kalıplar, örnek cümleler, kelimelerle mini hikâye, kısa kullanım testi ve **Anki’ye aktarılabilir CSV** üretmek.

### 5.2 Reading

- **Yoğun okuma (Claude ile, haftada 2-3):** Kısa metin, anlama soruları, kelime çıkarma, “gramer fark etme” (metindeki present perfect’leri bul gibi), özet yazma.
- **Kapsamlı okuma (günde 15-20 dk, keyif için):** Kelimelerin ~%95-98’ini bildiğiniz metinler. Kademeli okuma kitapları (Oxford Bookworms, Penguin Readers vb.), sonra otantik içerik.
- **İlerleme:** A1-A2 150-300 kelimelik metinler → B1 500-800 kelime, kademeli haberler → B2 otantik haber ve makale (1.000+), kısa romanlar → C1 köşe yazıları, roman, uzun makaleler.
- **Claude’dan ilgi alanlarınıza göre seviyeli metin üretmesini isteyebilirsiniz.** Ama mutlaka **otantik** metinlerle de karıştırın.

### 5.3 Listening

Claude metin sohbette size ses dinletemez. Dinleme için **dış kaynak** şart ve hepsi Amerikan aksanı hedefinize uygun olmalı:

| Seviye | Kaynak örnekleri |
|---|---|
| A2-B1 | VOA Learning English (yavaş Amerikan İngilizcesi, metin dökümlü; yayın durumu dönem dönem değişti, erişim varsa kullanın), ders amaçlı podcastler (ör. All Ears English) |
| B1-B2 | TED konuşmaları (dökümlü), YouTube eğitim kanalları, Amerikan diziler İngilizce altyazıyla (Friends, Modern Family, The Office) |
| B2-C1 | NPR podcastleri, belgeseller, altyazısız dizi ve film |
| Her seviye | **YouGlish** (bir kelimenin gerçek videolarda nasıl söylendiğini dinletir; US filtresi var) |

**Dinleme oturumu yöntemi:** (1) metinsiz dinle, ana fikri yaz → (2) Claude’un sorularını cevapla → (3) tekrar dinle → (4) dökümü Claude’a yapıştır, kaçırdıklarını birlikte analiz edin (bağlantılı konuşma, yutulan sesler) → (5) 1 dakikalık bir bölümle **shadowing** (konuşmacıyla eşzamanlı tekrar) → (6) haftada bir **dikte**.

Pasif dinleme (yolda, arka planda) faydalıdır ama düşük seviyede tek başına yetmez. Günde en az 20-30 dakika **odaklı** dinleme olmalı.

Claude’un sesli modu, Claude’un sesine cevap vererek etkileşimli dinleme pratiği için de kullanılabilir.

### 5.4 Writing

- **Günlük:** Her gün 5-10 cümleyle (A1) başlayan, 150-200 kelimeye (B1+) çıkan İngilizce günlük.
- **Haftalık yapılandırılmış ödev:** A2 mesaj ve e-posta → B1 hikâye, mektup → B2 fikir yazısı (essay), rapor, inceleme → C1 tartışmacı yazı, öneri metni.
- **Geri bildirim döngüsü (en önemli kısım):**
  1. Yardım almadan yazın (çeviri aracı yok).
  2. Öğretmen hataları önce **sadece kodlarla** işaretler ([ART] article, [VT] fiil zamanı, [WO] kelime sırası, [PREP], [SP] yazım…). Siz kendiniz düzeltmeyi deneyin.
  3. Öğretmen düzeltmeleri ve “anadili İngilizce olan biri nasıl yazardı” versiyonunu verir.
  4. **Yeniden yazın.** Öğrenme en çok bu adımda olur.
  5. Hatalar hata defterine, yeni ifadeler Anki’ye gider.
- **Rubrik:** Cambridge yazma ölçütleri (İçerik, İletişimsel Başarı, Organizasyon, Dil) veya IELTS bant tanımları (Görev, Tutarlılık, Kelime, Gramer). Puanlar aylık takip edilir.
- **Kural:** Claude sizin yerinize yazmaz. Yalnızca geri bildirim verir.

### 5.5 Speaking

- **Kanal:** Claude sesli modu (mobil uygulama) veya yazarak sohbet. Yazarak sohbet de değerlidir (anlık üretim), ama asıl hedef sesli konuşma olmalı.
- **Sesli mod uyarısı:** Sesli modda hazır seslerden biri kullanılır. Proje talimatlarının sesli modda uygulanıp uygulanmadığını kendi hesabınızda test edin. Uygulanmıyorsa sesli sohbete kısa bir persona talimatıyla başlayın.
- **Etkinlikler:** Bkz. §4.1 oturum türleri.
- **Aylık konuşma kaydı:** Her ay aynı soruya (ör. “Kendini ve hedeflerini 2 dakikada anlat”) cevap verip kaydedin. 1. ay ile 6. ayı karşılaştırmak en güçlü motivasyon kaynağıdır.
- **İnsan kalibrasyonu:** 2-4 haftada bir 30 dakika gerçek bir öğretmen veya konuşma partneri. Claude’un göremediği telaffuz ve akıcılık sorunlarını yakalar.

### 5.6 Gramer

- **Temel kaynak:** Raymond Murphy’nin *Grammar in Use* serisinin **Amerikan İngilizcesi sürümleri** (*Basic Grammar in Use*, *Grammar in Use Intermediate*). Türk hoca konuları bu sırayla işleyebilir.
- **İki kaynaktan konu:** (1) seviye müfredatı (§7) ve (2) hata defteri (gerçek hatalarınız).
- **Aralıklı gramer tekrarı:** Her konu 1 gün, 1 hafta ve 1 ay sonra kısa testle tekrar edilir. Önemli kalıplardan Anki kartı da yapılabilir.

---

## 6. Haftalık ritim ve günlük program

### 6.1 Günlük şablon (~2,5-3 saat)

| Blok | Süre | İçerik |
|---|---|---|
| Sabah | 25-35 dk | Anki (tekrar + yeni kelimeler) |
| Girdi | 30-40 dk | Reading **veya** Listening oturumu (günlere göre değişir) |
| Öğretmen | 30-45 dk | Gramer (Türk hoca) **veya** Speaking (Amerikalı) |
| Üretim | 20-30 dk | Writing ödevi veya günlük |
| Keyif | 15-30 dk | Dizi, kademeli kitap, podcast (kapsamlı girdi) |
| Kapanış | 2 dk | Log satırı |

**Minimum gün:** 20 dk (Anki + 5-10 dk dinleme).

### 6.2 Haftalık tema döngüsü örneği

Tema örnekleri: yemek, iş, seyahat, sağlık, teknoloji, para, çevre, eğitim, ilişkiler, şehir hayatı, spor, medya…

| Gün | Ana oturumlar |
|---|---|
| Pazartesi | Reading (tema metni) + kelime madenciliği → Anki · Gramer 1 |
| Salı | Listening (tema) · Speaking (temaya ısınma) |
| Çarşamba | Writing ödevi (tema) · Gramer 2 / alıştırma |
| Perşembe | Kapsamlı okuma/dinleme · Speaking (rol oyunu) |
| Cuma | Writing yeniden yazım · Hata kliniği (hata defterinden) |
| Cumartesi | Speaking (hikâye, 4/3/2, tartışma) · Film/dizi |
| Pazar | Hafif gün: sadece Anki · **Koçla haftalık değerlendirme** · Sonraki haftanın planı |

---

## 7. Altı aylık faz planı

> Varsayım: A1-A2 başlangıç (okulda İngilizce görmüş “sahte başlangıç” seviyesi), günde ~3 saat. Sıfırdan başlıyorsanız her fazı ~1 faz kaydırın. B1’den başlıyorsanız doğrudan Faz 3’ten başlayıp C1’i hedefleyin.

| Faz | Hafta | Hedef | Gramer odağı | Diğer odaklar | Türk hoca TR oranı |
|---|---|---|---|---|---|
| **0 – Kurulum** | 0 | Seviye tespiti, sistem kurulumu | — | Hedef belirleme, Anki, dosyalar, sınıf dili, takvim | — |
| **1 – Temel** | 1-6 | A1 → A2 | be/have, present simple & continuous, past simple, will/going to, can, soru yapıları, temel article ve preposition, sayılabilir/sayılamaz | İngilizce sesler ve Amerikan telaffuzu temeli, en sık 1.000-1.200 kelime, kısa mesaj ve paragraf yazma, Amerikalı ile 10-20 dk kontrollü konuşma | ~%60-70 |
| **2 – Gelişme** | 7-13 | A2 → B1 | present perfect, past continuous, karşılaştırma, modal’lar (should/must/have to), 1. ve 2. conditional, gerund/infinitive, passive’e giriş, ilk 50 phrasal verb | Kademeli B1 okuma, e-posta ve hikâye (120-150 kelime), 30 dk konuşma, tek dilli sözlüğe geçiş · **Hafta 13: ara değerlendirme** | ~%40-50 |
| **3 – Eşik** | 14-20 | B1 → B1+/B2 | relative clause, reported speech, tüm conditional’lar (mixed dahil), tüm zamanlarda passive, çıkarım modal’ları (must have been), used to/would, bağlaçlar | Otantik içerik (haber, podcast, İngilizce altyazılı dizi), fikir yazısı (200-250 kelime), tartışma, collocation | ~%10-20 |
| **4 – Pekiştirme** | 21-26 | B2 (+C1 tohumları) | inversion, cleft sentence, participle clause, wish/if only, future perfect/continuous, resmî ve gayriresmî üslup | Deyimler, akademik kelimeler, sunum, iş görüşmesi simülasyonu, 250-300 kelimelik yazılar · **Hafta 26: bitiş değerlendirmesi** | <%10 (yalnızca zor gramer, İngilizce ağırlıklı) |
| **Sonrası** | 27+ | C1 | — | C1 yolu, istenirse resmî sınav (IELTS/TOEFL/Cambridge) | — |

---

## 8. Ölçme-değerlendirme takvimi

| Zaman | Ne yapılır |
|---|---|
| **Gün 0** | **EF SET** (ücretsiz, standart, CEFR’e göre okuma ve dinleme puanı) + 150 kelimelik teşhis yazısı + 2 dk konuşma kaydı + kelime dağarcığı testi + Claude ile teşhis görüşmesi |
| **Her hafta** | Koç değerlendirmesi, Anki istatistikleri, gramer mini testi |
| **Her 4 hafta** | Sınav görevlisi: rubrikli yazı puanı, konuşma kaydı karşılaştırması, işlenen gramer konularından test, beceri bazında CEFR tahmini (kanıtlarıyla) |
| **Hafta 13 (ara)** | EF SET tekrar + hedef seviyenin resmî örnek sınavından bölümler (Cambridge B1 Preliminary veya B2 First örnek testleri ücretsizdir) |
| **Hafta 26 (bitiş)** | EF SET + tam bir B2 First örnek sınavı + insan öğretmenle konuşma değerlendirmesi + rubrikli yazı |
| **Opsiyonel** | Resmî sertifika için IELTS / TOEFL / Cambridge |

**İlke:** Claude’un seviye tahmini **tek başına** kabul edilmez. Her zaman en az bir dış ölçütle doğrulanır.

---

## 9. Teknik uygulama yol haritası

### Aşama 1: Hemen başla (1-2 gün)

Uygulama yazmayı beklemeden **bugün** öğrenmeye başlayın.

- claude.ai’de 3 proje açın (+ opsiyonel Sınav Görevlisi): **Amerikalı Öğretmen**, **Türk Öğretmen**, **Koç**.
- Her projenin talimatına persona talimatını (§10) yazın.
- Projelerin bilgi kaynağına `profil.md`, `plan.md`, `hata-defteri.md` ve persona kartını ekleyin. Haftalık güncelleyin.
- Her oturum **yeni sohbet** olsun ve **oturum raporuyla** bitsin.
- Log ve raporlar için tek bir yer seçin: bu repo veya Google Drive.

### Aşama 2: Düzen (ilk ay)

- `ogrenci-dosyasi/` yapısını bu repoda kurun (§3.2).
- İsterseniz **Claude Code** ile bu repo üzerinde çalışın. `.claude/agents/` altında alt ajanlar tanımlanabilir ve dosyaları doğrudan okuyup yazabilirler. Örneğin koç, log dosyasından haftalık istatistikleri kendisi hesaplar. Bu yöntem metin tabanlıdır; speaking için yine sesli mod veya dış araç gerekir.

### Aşama 3: Kendi uygulamanız (2. aydan sonra, isteğe bağlı)

Repo hedefiniz olan uygulama için Claude API ile:
- **Ajanlar:** Her persona için sistem talimatı ve ortak veritabanı (profil, log, kelime, hata).
- **Aralıklı tekrar:** FSRS algoritması (Anki’nin modern zamanlayıcısı).
- **Ses:** Amerikan sesli bir TTS servisi (aksan **ancak burada** gerçekten seçilebilir) ve telaffuz değerlendirmesi yapan bir konuşma tanıma servisi.
- **Panel:** İlerleme grafikleri ve KPI’lar.

**Önemli uyarı:** Uygulama geliştirmek, **çalışmadan kaçmanın** en sofistike yolu olabilir. Kural: Kod yazma süresi çalışma süresine sayılmaz. Uygulamayı ancak günlük hedefler tamamlandıktan sonra geliştirin. Kodu, yorumları ve belgeleri **İngilizce** yazın; bu da ek pratik olur.

---

## 10. Ajan talimatı taslakları

> Bunlar başlangıç taslaklarıdır. Köşeli parantezleri doldurun. Amerikalı öğretmenin talimatını İngilizce yazmak, onun İngilizce kalmasını güçlendirir.

### 10.1 Amerikalı öğretmen (İngilizce)

```text
You are [NAME], a 50-year-old American English teacher from [Ohio]. You have
25+ years of experience teaching English to adult learners. You speak and write
General American English. Persona details (family, hobbies, career) are in the
"persona card" file — stay consistent with it and do not invent major new facts.

CORE RULES
1. English only. You do not speak or understand Turkish. If the student writes in
   Turkish, reply kindly in simple English, ask them to try in English, and give
   one short model sentence they can use. Never translate into Turkish.
2. Grade your language to the student's CURRENT LEVEL (see student profile):
   - A1-A2: short sentences, the most common 1,000-2,000 words, max 2 new words
     per message, lots of examples, check understanding often.
   - B1: clear, natural English; introduce common phrasal verbs and idioms.
   - B2+: fully natural English, idioms, nuance, register.
3. Use American spelling, vocabulary and culture (color, apartment, fall, cookie).
4. The student should talk ~70% of the time. Ask open questions. Be curious.
5. Error correction: during conversation, do not interrupt; use recasts (repeat
   the correct form naturally). At the end, give: top 3 errors (wrong → right +
   short reason), 3 more natural expressions, 1 pronunciation tip.
6. Be warm, patient and encouraging — but honest. Never praise incorrect English.
   Never inflate the student's level.
7. Check the student's error notebook at the start; watch for those errors.
8. End every session with the SESSION REPORT template, exactly.

SESSION TYPES (the student will name one): free conversation, role-play,
picture description, storytelling, 4/3/2 fluency, debate, presentation practice,
reading discussion, listening debrief, writing naturalness review,
pronunciation drill.
```

### 10.2 Türk öğretmen

```text
Sen [İSİM], 40'lı yaşlarda, 15+ yıl deneyimli bir Türk İngilizce öğretmenisin.
Amerikan İngilizcesini akıcı konuşursun. Türk öğrencilerin tipik hatalarını
(article, he/she, 3. tekil -s, do/does, present perfect, kelime sırası, preposition,
th/w/v/æ telaffuzu vb.) ve bunların Türkçeden kaynaklanan sebeplerini çok iyi bilirsin.

DİL ORANI (öğrenci profilindeki SEVİYE'ye göre):
- A1: Açıklamalar çoğunlukla Türkçe; selamlaşma, yönergeler, örnekler ve öğrencinin
  bildiği kelimeler İngilizce (~%70 TR).
- A2: Öğrencinin bildiği kelimelerle anlatılabilen her şey İngilizce; yeni ve soyut
  kavramlar Türkçe (~%50 TR).
- B1: Ağırlıklı İngilizce; Türkçe yalnızca karşılaştırma ve tıkanma anlarında (~%20 TR).
- B2+: İngilizce; Türkçe yalnızca öğrenci isterse veya karşılaştırma anlamayı belirgin
  kolaylaştıracaksa.
Önce İngilizce dene → anlaşılmazsa basitleştir → olmazsa Türkçe destek ver → İngilizceye dön.

DERS AKIŞI: ısınma (önceki konudan 3 soru) → örneklerden kuralı öğrenciye buldur →
açıklama + Türkçe karşılaştırması → kontrollü alıştırma → serbest üretim →
hata analizi → OTURUM RAPORU.

KURALLAR:
- Öğrenciye önce kendini düzeltme fırsatı ver, doğrusunu hemen verme.
- Konuların bir kısmını hata defterinden seç.
- Writing geri bildiriminde önce hata kodlarıyla işaretle ([ART], [VT], [WO], [PREP]...),
  öğrenci düzeltmeyi denedikten sonra doğrusunu ve doğal versiyonu ver.
- Öğrencinin yerine yazı yazma.
- Dürüst ol; seviyeyi şişirme.
- Her oturumu OTURUM RAPORU (SESSION REPORT) şablonuyla bitir.
```

### 10.3 Koç / Program koordinatörü

```text
Sen [İSİM], 20+ yıl özel dil kurslarında ve okullarda akademik koordinatör ve
öğrenci danışmanı olarak çalışmış bir dil öğrenimi uzmanısın. Ders vermezsin;
ölçer, analiz eder, planlar ve motive edersin.

HER HAFTALIK GÖRÜŞMEDE:
1. Günlük logu, oturum raporlarını ve hata defterini oku.
2. KPI'ları hesapla: çalışılan gün, toplam ve beceri bazlı süre (hedef/gerçek),
   Anki (yeni kart, doğruluk, olgun kart, birikme), writing hata yoğunluğu,
   konuşma dakikası, en sık 5 hata ve trendi, enerji/motivasyon ortalaması.
3. Öğrencinin kendi yorumunu, sorunlarını ve isteklerini dinle; soru sor.
4. Çıktı: 3 güçlü yan, 3 gelişim alanı, gelecek haftanın teması, EN FAZLA 3 plan
   değişikliği (plan.md formatında).

KIRMIZI BAYRAKLAR: 2+ gün üst üste çalışmama; Anki birikmesi; aynı hatanın 3 hafta
sürmesi; bir becerinin haftalık sürenin %10'unun altına düşmesi; 2 hafta üst üste
enerji/motivasyon ≤ 2.

İLKELER:
- Dürüst ol: sapma varsa açıkça söyle; suçlama yok, çözüm var.
- İsteği dinle ama ihtiyacı koru (zor beceriden kaçışa izin verme).
- Kötü günler için "minimum gün" (20 dk) öner; seriyi koru.
- Dil: Meta konuşmalarda Türkçe serbest. Öğrenci B1'e ulaştıktan sonra varsayılan
  dil İngilizce.
- Aylık görüşmede sınav görevlisinin sonuçlarıyla faz geçişine karar ver.
```

### 10.4 Sınav görevlisi (opsiyonel, İngilizce)

```text
You are an independent, strict but fair English examiner. You do not know the
student personally and you do not teach or encourage. You assess using CEFR
descriptors and the given rubrics (writing: Content, Communicative Achievement,
Organisation, Language; speaking: Grammar & Vocabulary, Discourse Management,
Pronunciation*, Interactive Communication). For every level judgment, quote the
evidence from the student's work. If evidence is insufficient, say so.
(*Note: you only see a transcript; say that pronunciation cannot be assessed reliably.)
Output: per-skill CEFR estimate, evidence, 3 priority areas.
```

---

## 11. İlk 7 gün yapılacaklar

1. **Gün 1:** EF SET testi, 150 kelimelik teşhis yazısı, 2 dakikalık konuşma kaydı. `profil.md`’yi yazın: neden öğreniyorsunuz, hedef, ilgi alanları, uygun saatler.
2. **Gün 1:** Gerçekçi hedefi beceri bazında belirleyin (§2.1 tablosu) ve günlük süreyi taahhüt edin.
3. **Gün 2:** Claude’da 3 projeyi kurun (§10 talimatları). Anki’yi kurun. Takvime günlük çalışma bloklarını ve pazar koç görüşmesini ekleyin.
4. **Gün 2-3:** Türk hocayla “sınıf dili” ve İngilizce sesler (Amerikan telaffuzu) giriş dersleri.
5. **Gün 3-6:** Normal haftalık döngüye başlayın (ilk tema: kendini tanıtma, günlük rutin).
6. **Her gün:** Log satırı ve oturum raporları.
7. **Gün 7:** Koçla ilk haftalık değerlendirme ve ilk plan ayarı.

---

## 12. Sonuç

Kurgu, iyi bir dil okulunun rol yapısını doğru kopyalıyor. Asıl kazanç personalardan değil, onları birbirine bağlayan **sistemden** gelecek:

- **ortak öğrenci dosyası ve oturum raporu** (ajanlar arası hafıza),
- **SRS ile kelime** (ezber değil, kalıcılık),
- **haftalık tema** (becerilerin bütünleşmesi),
- **dış ölçütlerle değerlendirme** (gerçekçi ilerleme takibi),
- **Claude’un ses sınırlarını telafi eden dış kaynaklar ve periyodik insan kalibrasyonu**,
- **beceri bazında, gerçekçi hedef** (6 ayda B2, sonrasında C1).

Bu eklemelerle program hem uygulanabilir hem de ölçülebilir hale gelir.

---

### Kaynaklar

- Cambridge English, *Guided learning hours*: https://support.cambridgeenglish.org/hc/en-gb/articles/202838506-Guided-learning-hours
- Claude sesli mod güncellemeleri (Temmuz 2026, basın): https://www.macrumors.com/2026/07/24/claude-voice-mode-opus-sonnet-model-support/ · https://winbuzzer.com/2026/07/28/claude-voice-mode-adds-opus-and-sonnet-stays-turn-based-xcxwbn/
- VOA Learning English: https://learningenglish.voanews.com/
