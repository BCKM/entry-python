# 4.3 Voqeaga asoslangan (Event-Driven)

Keling, **voqeaga asoslangan yoki voqeaga yo‘naltirilgan dasturlash paradigma**si (Event-Based) haqida gaplashamiz. Ushbu paradigma keng qo‘llanila boshlagan davr operatsion tizimlar (OS: Operating System) interfeyslari **konsol** (Console) matnli buyruqlari orqali ishlashdan **grafik foydalanuvchi interfeysi** (GUI: Graphic User Interface)ga o‘tish davriga to‘g‘ri keladi. Boshqacha aytganda, GUI muhitiga mos dasturlar kerak bo‘ldi, va dastur ishlab chiqish usullari ham shu ehtiyojlarga mos ravishda rivojlandi. **GUI muhiti** deganda grafik asosida ishlaydigan tizim tushuniladi. Masalan, kompyuter yoki smartfonlarda biz bosish yoki teginish orqali tanlovlar va boshqaruvlar amalga oshiramiz. Bugungi kunda bu kompyuterni boshqarishning keng tarqalgan usuli bo‘lib, ushbu paradigmadan foydalanishni tushunish qiyinchilik tug‘dirmaydi. Shunga qaramay, voqeaga yo‘naltirilgan dasturlash konsepsiyasini quyidagi rasm yordamida yaxshiroq tushunishga harakat qilaylik.

<figure><img src="../.gitbook/assets/eventdriven.png" alt="" width="563"><figcaption><p>Manba: <a href="https://kamang-it.tistory.com/entry/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D-%ED%8C%A8%EB%9F%AC%EB%8B%A4%EC%9E%84%EC%9D%B4%EB%B2%A4%ED%8A%B8-%EA%B8%B0%EB%B0%98-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8DEvent-based-programming">Kamang's IT Blog</a></p></figcaption></figure>

**Hozir ekranda ko‘rinib turgan dasturimda biror harakatni qo‘zg‘atuvchi (trigger) barcha holatlar voqea (event) deb ataladi. Masalan, foydalanuvchi ekranda ma'lum bir rasmli tugmani yoki belgini bosgan payt, klaviaturada ma'lum bir tugmachani (harf, maxsus belgi, yo‘nalish tugmalari va boshqalar) bosgan payt, sichqonchaning ma'lum bir tugmachasini (chap, o‘rta, o‘ng) bosgan payt, belgilangan vaqtga yetgan payt yoki boshqa bir dastur mening dasturimni chaqirgan payt va shunga o‘xshash holatlar.**

Ya'ni, dasturchi bunday voqealar sodir bo‘lishini oldindan taxmin qilib, har bir voqea sodir bo‘lganda qaysi vazifani bajarish kerakligini ko‘rsatadigan tarzda kod yozishni **voqeaga asoslangan dasturlash paradigam**si deb atash mumkin. Biz allaqachon Entry platformasida shu usulda kod yozish tajribasiga egamiz, shuning uchun ushbu tushunchani anglash yoki amalda qo‘llashda qiyinchilik bo‘lmaydi, deb o‘ylayman. Faqatgina, Entry-Python da bu kabi voqealar uchun qanday funksiyalardan foydalanish kerakligini bilishimiz kifoya.

Quyidagi jadvalda Entry da mavjud bo‘lgan voqealar turlari va ushbu voqealarga mos keladigan, oldindan aniqlangan (kelishilgan) **kolbek(callback) funksiyalar** ([3.1-bo‘limdagi kolbek funksiyalarga qarang](../boshlash/hello_world.md#kolbek-callback-funksiyasi-nima)) ro‘yxatini ko‘rishingiz mumkin.

| Voqea turi                              | Blokli kodlashdagi bloklar                                               | Matnli kodlash uchun kolbek funksiyasi |
| --------------------------------------- | ------------------------------------------------------------------------ | -------------------------------------- |
| Ekrandagi boshlash tugmasini bosganda   | <img src="../.gitbook/assets/bosh.png" alt="" data-size="original">      | def when\_start():                     |
| Klaviaturadagi tugmacha bosilganda      | <img src="../.gitbook/assets/klav (1).png" alt="" data-size="original">  | def when\_press\_key("q"):             |
| Sichqoncha bosilganda                   | <img src="../.gitbook/assets/sich (1).png" alt="" data-size="original">  | def when\_click\_mouse\_on():          |
| Sichqonchani bosishni qo‘yib yuborganda | <img src="../.gitbook/assets/sichq (3).png" alt="" data-size="original"> | def when\_click\_mouse\_off():         |
| Obyektni bosganda                       | <img src="../.gitbook/assets/obb (2).png" alt="" data-size="original">   | def when\_click\_object\_on():         |
| Obyektni bosishni qo‘yib yuborganda     | <img src="../.gitbook/assets/obbq (1).png" alt="" data-size="original">  | def when\_click\_object\_off():        |
| Yangi sahna boshlanganda                | <img src="../.gitbook/assets/sb (1).png" alt="" data-size="original">    | def when\_start\_scene():              |

