# 3.1 "Hello World" namuna kodini tushunish

Agar boshqa turdagi kompyuter dasturlash tillari kitoblarini o‘qib ko‘rgan bo‘lsangiz, [ekranda "Hello World!" degan oddiy jumlani chiqaruvchi kod misoli](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program) bilan boshlanishini ko‘rgan bo‘lishingiz mumkin. Biz ham ushbu odatiy misol koddan boshlab, grammatikani o‘rganishni boshlaymiz.

{% tabs %}
{% tab title="Ijro narijasi" %}
<figure><img src="../.gitbook/assets/image (4).png" alt="" width="311"><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Blokli kodlash" %}
<figure><img src="../.gitbook/assets/entry FEQ.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Entry-Python" %}
{% code lineNumbers="true" %}
```python
# Entrybot's Python code

import Entry

def when_start():
    Entry.print("Hello World!")
```
{% endcode %}
{% endtab %}
{% endtabs %}

Kelgusida kod tahlili yuqoridagi kabi 3 ta yorliq shaklida tuziladi: birinchi yorliq kodning bajarilish natijasini ko‘rsatadi, ikkinchi va uchinchi yorliqlarda esa bir xil bajarilish natijasini olish uchun Entry-Python va blokli dasturlash shaklidagi kodlarni taqqoslash imkoniyati yaratiladi.

Ushbu misolda bu juda oddiy dastur bo'lib, uni blok kodlashda faqat ikkita blok <img src="../.gitbook/assets/entry FEQ (2).png" alt="" data-size="original"> bilan kodlash mumkin. Biroq, Entry-Python bilan kodlaganda, u 6 qatordan iborat uzun kodga aylanadi (kodni o'qishni yaxshilash uchun o'rtaga kiritilgan bo'sh qatorlar ham hisobga olingan). Men hozir bu misolni o'zingiz yozishingizni tavsiya etmayman. Keyinchalik kodlash uchun ko'plab imkoniyatlarga ega bo'lasiz va birinchi navbatda matn kodlash misoli sifatida eng oson kod deb ataladigan ushbu 6 qatorning ma'nosini aniq tushunish muhimroqdir. Shuning uchun men ushbu tarkibni hozircha blok kodlash bilan kodlashni tavsiya qilaman va keyin uni Entry-Python kodiga aylantirish uchun menyuda avtomatik kod o'zgartirish menyusini tanlang.

🔢 **1-qatordagi** "_# Entrybot's Python code_" nimani anglatadi? **Matnni kodlashda siz har bir belgi, hatto ba'zan bo'sh joy ham ma'no va maqsadga ega ekanligini bilasiz**. Demak, 1-qatorda birinchi bo'lib paydo bo'lgan **#** belgisi ham ma'no va maqsadga ega ekanligini xulosa qilishimiz mumkin va uni joriy **#** belgisidan keyin yozilgan tarkibdan xulosa qilishimiz mumkin. Bu "Ushbu belgidan boshlab va undan keyin (lekin bir qator ichida) yozilgan hamma narsani izoh (comment) deb hisoblang" degan ma'noni anglatadi.

Matnli kodlashda **izoh (comment)** degan tushunchaning ma’nosini tushunib olaylik. Kompyuter biz yozgan kodni yakuniy bajarish uchun bosqichma-bosqich o‘qib chiqadi. Ammo kodda izoh qismiga duch kelganda, uni bajarish jarayoniga hech qanday aloqasi yo‘qligi sababli uni o‘qimay, e’tibordan chetda qoldirishi kerakligi haqida bizdan “xabar” oladi. Shu bois, kompyuter ushbu qismni o‘qishdan voz kechib, uni chetlab o‘tadi (skip).

Xo‘sh, **izoh nima uchun kerak?** **Uning ikkita asosiy maqsadi bor**: birinchisi, izohning nomi o‘zi aytib turganidek, yozilgan kodni tushuntirishdir. Ya’ni, qo‘shimcha ma’lumot berish orqali keyinchalik muallifning o‘zi yoki bizning hamkasblarimiz ushbu kodni ko‘rib, uni tez va to‘g‘ri tushunishiga yordam berish uchun ishlatiladi. Ikkinchisi, kodda mantiqiy xatolarni (sintaksis xatolar emas, balki bajarilganda kutilganidek ishlamaydigan xatolarni) tuzatish (Debugging – xatolarni topish va tuzatish jarayoni) jarayonida ishlatiladi. Bu jarayonda, kodning bir qismini vaqtincha izoh sifatida belgilab, uni bajarishdan chetda qoldirish (skip qilish) orqali xatoni tezroq aniqlash uchun ishlatiladi.

🔢 Endi **2-qator** tahliliga o‘tamiz. Bu qator oddiygina bo‘sh qoldirilgan. Bunday qatorlar 2- va 4-qator bo‘lib, umumiy ikki qatorni tashkil etadi. Nega bo‘sh qator kiritilgan? Sababi juda oddiy. Kompyuter uchun kodni tahlil qilishda hech qanday ahamiyatga ega emas, lekin biz, insonlar, kodni o‘qiganimizda uni yaxshiroq va tushunarliroq qilish uchun kiritiladi. Garchi hozir matnli kodlashni endigina boshlayotganimiz bois buni yaxshi anglamasakda, dasturlashning bir oz kattaroq loyihalariga o‘tganimizda, odatda yakkama-yakka emas, balki boshqa dasturchilar bilan hamkorlikda ishlashimiz kerak bo‘ladi. Shu bois, boshqa odamlar sizning kodingizni oson, tez va qulay o‘qiy olishi uchun doim e’tiborli bo‘lish odatini rivojlantirish muhimdir. Bu dasturchilar uchun zarur bo‘lgan asosiy fazilatlardan biridir. Shuning uchun kod yozishda tegishli bo‘sh qatorlardan foydalanish va tegishli joyda izoh kiritish juda muhim.

🔢 Endi **3-qatorga** o‘tamiz. Unda _**import Entry**_ degan ikki so‘z bor. Bu jumlada **import** kalit so‘zining ma’nosi – biz kod yozayotgan faylga tashqi manbadan kutubxonani (Libriary, Python-da paket(Package), undan kichikroq birlik – modul(Module) deb ataladi) olib kelib, undan foydalanishni bildiradi. **import** dan keyin keladigan **Entry** so‘zi esa bizga kerak bo‘lgan kutubxonaning nomi. Ushbu kodning umumiy ma’nosi shundan iboratki, **Entry** (kutubxonaning nomi kutubxona muallifi tomonidan beriladi) deb nomlangan kutubxonani tashqi manbadan chaqirib olib foydalanishimiz kerak. Endi kutubxona nima ekanligini bilib olish vaqti keldi.

## Kutubxona nima?

{% hint style="info" %}
**Kutubxona (Library):**[ Dasturiy ta’minotni ishlab chiqish](https://en.wikipedia.org/wiki/Software_development)da [kompyuter dasturi ](https://en.wikipedia.org/wiki/Computer_program)tomonidan foydalaniladigan[ o'zgarmas resurslar](https://en.wikipedia.org/wiki/Non-volatile_memory) to'plami. Bunga konfiguratsiya ma’lumotlari, hujjatlar, yordamchi materiallar, xabarlar shablonlari, [oldindan yozilgan kodlar](https://en.wikipedia.org/wiki/Code_reuse), [subrutinlar ](https://en.wikipedia.org/wiki/Function_\(computer_programming\))(funksiyalar), [sinf](https://en.wikipedia.org/wiki/Class_\(computer_programming\))lar, [qiymat](https://en.wikipedia.org/wiki/Value_\(computer_science\))lar va [ma’lumot turlari](https://en.wikipedia.org/wiki/Data_type) spetsifikatsiyasi kiradi.

**Manba:** Vikipediya
{% endhint %}

Yuqoridagi kutubxona ta’rifini o‘qib tushundingizmi? **Kutubxonani oddiy qilib tushuntiradigan bo‘lsak, bu dasturchilar tomonidan dasturlarni tez va qulay ishlab chiqish maqsadida oldindan yozib qo‘yilgan kodlar to‘plami (asosan funksiyalar, sinflar, o‘zgaruvchilar va boshqalar)** deb aytish mumkin. Siz allaqachon Entry’da funksiyalardan (Function) foydalanib ko‘rgansiz va funksiyaning maqsadini yaxshi tushunasizmi? Funksiyaning asosiy maqsadi nima edi? Bir nechta joyda takroran ishlatiladigan kod qismlarini funksiya sifatida ajratib yozib qo‘ysak, keyinchalik ushbu funksiya blokini bir marta chaqirish orqali xohlagan vazifamizni osongina bajarishimiz mumkin bo‘ladi. Natijada kodlash jarayoni sezilarli darajada soddalashadi, kod samaradorligi oshadi va funksiyalar tufayli soddalashtirilgan kod butun dasturning tushunilishini sezilarli darajada yaxshilaydi.

Bundan tashqari, **funksiyaning yanada foydali va asosiy maqsadi — yaxshi yozilgan funksiyani dasturdagi turli joylarda (bitta obyekt yoki ko‘p sonli obyektlar ichida) bir necha marta ishlatishdir (buni kodni qayta ishlatish deyishadi). Bu dastur bir marta yozilib tugatilmay, balki doimiy ravishda yangilanish va rivojlanish jarayonini boshdan kechiradigan tirik mavjudot kabi bo‘lgani sababli, keyingi o‘zgarishlarga osonlik bilan moslashishga imkon beradi.** Chunki biror funksiyani alohida bir vazifa uchun ajratib, yozib qo‘yganingizdan keyin, o‘sha funksiyaning mazmunini yaxshilash yoki o‘zgartirish kerak bo‘lsa, ushbu funksiyadan foydalanilgan barcha kodlarda o‘zgarishlar bir vaqtning o‘zida avtomatik ravishda tatbiq etiladi.

Agar hozirda funksiyaning maqsadi va uning mazmunini to‘liq tushunmagan bo‘lsangiz, ehtimol siz Entry blokli kodlashda funksiyalardan foydalanib ko‘rmagan yoki funksiyaning maqsadini yaxshi tushunmasdan foydalangan bo‘lishingiz mumkin. Bu yerda funksiya haqida qayta tushuntirish bu kitobning doirasiga kirmaydi, shuning uchun kimga kerak bo'lsa [video havola](https://youtu.be/XRBg448VYzU?si=zQhbsR4d0jx9Mm2_)ni qoldiraman, ularni o‘zlari mustaqil ravishda o‘rganishlari mumkin.

Agar bir yaxshi yozilgan funksiyaning qanchalik foydali ekanligini tajribada ko‘rgan bo‘lsangiz, endi shunday savol tug‘ilishi mumkin: "Bu funksiyani faqat o‘zim ishlata olishim juda achinarli emasmi? Buni barcha dasturchilar, kichikroq miqyosda mening hamkasblarim yoki butun dunyo dasturchilari ham ishlatsa, bu yanada foydali bo‘lmaydimi?" Shunday qilib, yaxshi yozilgan va foydali funksiyalarni hammaga ochiq tarzda ishlatish mumkin bo‘lgan tizim yaratildi, bu tizim _kutubxona_ (yoki paket) deb ataladi. Dasturchilar ayniqsa bunday narsalarga juda qiziqishadi. Chunki ular asosan yuqori samaradorlikka intiluvchilardir; birinchi, alohida funksiyalarni bir joyga to‘playdilar, keyin ularni yana kattaroq bir tuzilma ostida birlashtiradilar. Buni grafik ko‘rinishda tasvirlasak, quyidagicha ko‘rinadi.

<figure><img src="../.gitbook/assets/image (1) copy.png" alt=""><figcaption></figcaption></figure>

_Kutubxona (library) tushunchasini tushuntirish uchun osonroq va mosroq taqqoslash haqida o‘ylaganimda, uning nomi bejiz tanlanmagan bo‘lsa kerak. Chunki bu aynan kitoblar bilan to‘lgan kutubxonaga o‘xshaydi. Kutubxonada ayrim alohida kitoblar mavjud (bularni modul deb tasavvur qilish mumkin), ba’zan esa ketma-ketlikdagi kitoblar to‘plamlari ham uchraydi (buni paket deb qarash mumkin). Kitobning ichida esa mazmunni tashkil etuvchi boblar, bo‘limlar, paragraflar va jumlalar bor. Bu tuzilmalarni klasslar, funksiyalar va o‘zgaruvchilar bilan taqqoslash ham o‘rinli._

_Hozircha, kutubxona ichida biz uchun oldindan boshqalar tomonidan ishlab chiqilgan foydali kod to‘plamlari (asosan funksiyalar) bor, biz esa ularni olib, kodlash jarayonida foydalanamiz, deb bilib qo‘ysangiz yetarli._

🔢 Nihoyat, biz **5-qator**ga yetdik. Buni kod tahlilining oxiri deb xisoblashingiz mumkin. Buning sababi shundaki, 5 va 6 qatorlar alohida kodlar emas, balki bitta ma'noga ega bo'lgan kodlar to'plamidir.

```python
def when_start():
    Entry.print("Hello World!")
```

_**def when\_start():**_ Bu kod nimani anglatadi? Bu avval bir necha marta aytib o'tilgan funksiyani bevosita yaratuvchi koddir. Biz boshidanoq funksiyani ishlatish uchun uni tashqaridan chaqirishni o'rgandik va endi uni o'zimiz yaratishni ham o'rganyapmiz! Matnli kodlashda funksiya shu qadar muhim. Birinchidan, Python matn kodlashda funksiya yaratish uchun umumiy grammatikani o'rganamiz.

## Funksiyani qanday yaratish (ta'riflash)

<figure><img src="../.gitbook/assets/image (2).avif" alt="" width="375"><figcaption></figcaption></figure>

Yuqoridagi standart sintaksisning har bir so‘z va belgilarining ma’nosini tushunib chiqaylik. _Funksiya yaratish uchun har doim qator boshida def (definition – "ta’rif"ning qisqartmasi) kalit so‘zi bilan boshlash kerak._ Bu so‘z "endi yozadigan narsalarim funksiya yaratish (ta’riflash(definition)) jarayoni" degan ma’noni bildiradi. Keyin, yaratmoqchi bo‘lgan funksiyaga ma’noli va o‘zingizga qulay nom berish kerak. Shundan so‘ng, funksiya chaqirilganda chaqiruvchidan olinadigan qiymatlar (bular dasturlash dunyosida "parametr" deb ataladi) qavs ichida vergul (`,`) bilan ajratilgan holda yoziladi. Va nihoyat, (`:`)belgisi bilan funksiya qobig‘i tugallanganini ko‘rsatib, keyingi qatordan funksiya ichida bajarilishi kerak bo‘lgan haqiqiy kodlar yozilishi boshlanishi kerakligini bildiradi.

_**def when\_start():**_  yuqoridagi standart sintaksisga yana bir bor murojaat qilib tushuntiradigan bo‘lsak, bu `when_start` nomli funksiya yaratilayotgani va bu funksiya hech qanday qiymat (parametr) qabul qilmasligi (shuning uchun qavs ichida hech narsa yo‘q) bildiradi.

🔢 Endi oxirgi, ya’ni **6-qator**ga o‘tamiz. Bu yerda funksiya chaqirilganda bajarilishi kerak bo‘lgan kod yoziladi. Qiziq tomoni shundaki, boshqa qatorlardan farqli o‘laroq, bu qator boshlanishidan oldin ma’lum miqdorda bo‘sh joy qoldiriladi (bu bo‘shliqni **Tab** tugmasini bir marta bosish yoki **Spacebar** tugmasini to‘rt marta bosib hosil qilish mumkin). Dasturlash dunyosida bo‘shliq ham ma’noga ega ekanligi haqida ilgari gaplashgan edik. Bu xuddi shunday holatlardan biri bo‘lib, Python standart sintaksisiga ko‘ra bo‘shliq maqsadli ishlatiladi. Bu nafaqat funksiyalarda, balki boshqa ko‘plab kodlarda ham qo‘llaniladi. Shu sababli, boshidanoq uni yaxshilab o‘rganib olish muhimdir. **Bu bo‘shliqning ma’nosini oddiy qilib tushuntirsak: har bir qatorda bir xil miqdorda bo‘sh joy qoldirilishi bilan, o‘sha satrlar bir kod blokiga tegishli ekanligini ko‘rsatish uchun ishlatiladi.**

Buni bizning kodimizga taqqoslaydigan bo‘lsak, **when\_start** funksiyasiga tegishli bo‘lgan kodning qayerdan qayergacha ekanligini kompyuterga bildirish uchun bo‘sh joy ishlatilgan. Hozirgi kunda bu funksiya chaqirilganda faqat bitta qator kodni bajaradigan juda oddiy funksiya bo‘lgani sababli bu gapni tushunish qiyin bo‘lishi mumkin. Lekin kelajakda ko‘proq kodlarni bajaradigan va bajarish tarkibi uzun bo‘lgan funksiyalarni ko‘rganingizda, bu bo‘shliqning ma’nosi yanada yaqqolroq bo'ladi.

Endi _**Entry.print("Hello World!")**_ kodini tahlil qilamiz. Uni qismlarga ajratsak: **Entry** — bu kutubxona nomi, undan keyin nuqta (`.`) qo‘yilgan, so‘ngra esa _**print("Hello World!")**_ yozilgan. Oldin aytganimizdek, dasturlashda nuqta (`.`) ham o‘ziga xos ma’noga ega. Agar kutubxona nomidan keyin nuqta qo‘yilsa, bu o‘sha kutubxona ichidagi narsalarni (masalan, funksiyalar, klasslar, o‘zgaruvchilar va boshqalar) ishlatishni anglatadi. Bu holda _**print("Hello World!")**_ — **Entry** kutubxonasi ichida joylashgan funksiyadir. Shu sababli, 1-qatorda import orqali olib kelingan **Entry** kutubxonasidagi **print** funksiyasini chaqirayotganimizni bildiradi.**print** nomidan xulosa qilganimizdek, u ekranga ma’lum bir qiymatni chiqarish uchun ishlatiladi. Ekranga chiqariladigan mazmun esa, `"` (qo‘shtirnoq) ichida yoziladi. Bu qo‘shtirnoqlar ekranda ko‘rsatiladigan matnning boshlanishi va tugashini aniqlab beradi. Masalan, bu kodda "Hello World!" ekranga chiqariladi.

Xo‘sh\~ mana shunday qilib 6 qatorlik juda oddiy dastur kodi tahlili nihoyasiga yetdi! O‘zingizni yengil his qilyapsizmi? Endi, agar siz Entry da “Boshlash” tugmasini bossangiz, o‘sha 6 qatorlik kod ishga tushadi va ekranda biz xohlagan natija, ya’ni **"Hello World!"** yozuvi paydo bo‘ladi. Hammasi yaxshi ishlaydi. Kod to‘liq tushuntirildi va muvaffaqiyatli bajarildi. Shunga qaramay, sizda nimadir yechimsiz qolayotgandek yoki qandaydir javobsiz savollar qolayotgandek tuyilishi kerak. Sizda bu his qoldimi? Agar qolmagan bo‘lsa ham, xafa bo‘lmang.&#x20;

Qolgan savol shundan iboratki, bizning shu 6 qatorlik kodimizda qanday qilib istalgan natijani olish mumkin? Aslida, natija chiqishi uchun kod to‘liq emas. Albatta, kodning boshqa qismi bo‘lishi kerak edi. Biz **when\_start** funksiyasini faqat ta'rifladik, ammo uni ishlatish uchun chaqirgan kodni hech qayerda ko‘rmayapmiz. Ya'ni, **when\_start** funksiyasini kodingizda bir joyda chaqirishingiz kerak va faqat shunday qilib, chaqirilgan funksiyaning bajarilishi bilan ekranda chiqishi amalga oshadi. Biroq, bizning 6 qatorlik dasturda hech qayerda **when\_start** funksiyasini bevosita chaqiradigan kod yo‘q. Shunda, bu funksiyani kim va qanday chaqirib, qanday qilib ishga tushirdi?

## Kolbek (callback) funksiyasi nima?

Javobni aytadigan bo'lsak, bizning dasturimizdagi funksiyani to'g'ridan-to'g'ri chaqirmagan bo'lsak ham, bizning dasturimizdan tashqarida, ya'ni tashqi tomondan ushbu funksiya chaqirilgan. Demak, kim chaqirdi? Ha, chaqiruvchi Entry dasturini o'zidir. Entry bizning **when\_start** funksiyamizni avtomatik ravishda chaqirgan. Bu yerda umumiy ma'lumot sifatida bilish kerak bo'lgan bir atama mavjud. Agar funksiya bo‘lsa-yu, lekin uni men bevosita chaqirmasdan, tashqi tizim tomonidan biror vaqtda avtomatik tarzda chaqirilsa, bunday funksiyani kolbek (callback - so'zma so'z tarjimasi "qayta chaqirish") funksiyasi deb ataladi. Ha, **when\_start** kolbek funksiyasi edi. Bunday kolbek funksiyalarining nomini biz o'zimiz xohlagancha belgilay olmaymiz. Entry o'zi oldindan belgilab qo'ygan funksiya nomlarini ishlatishimiz kerak. Ya'ni, Entry ichida qandaydir kelishuv bor, ya'ni foydalanuvchi "Boshlash" tugmasini bosgan zahoti, Entry ichida doimo **when\_start** funksiyasini chaqirishi uchun dasturlangan. Agar bu gapga ishonmasangiz, **when\_start** nomini bilvosita o'zgartirib, "Boshla" tugmasini bosing. Kutgan xatti-harakat amalga oshadimi? Biz kutgandek ishlamaydi. Chunki bizning dasturimizda oldindan belgilangan va mavjud bo'lishi kerak bo'lgan o'sha **when\_start** funksiyasi yo'q.

Faqatgina 6 qatorlik kichik dastur bo'lsada, matnli kodlashning ko'plab asosiy jihatlarini tushunish uchun yaxshi misol ekanligi shubhasiz. Keyingi bosqichda dasturlashning asosiy elementlarini (ketma-ketlik, takrorlash, shartlar va boshqalar) birma-bir o'rganib chiqamiz.
