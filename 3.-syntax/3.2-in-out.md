# 3.2 Kiritish/Chiqarish (Input/Output)

Dasturda kiritish/chiqarish nima? Bu foydalanuvchidan kerakli ma'lumotlarni olish yoki aksincha, ko'rsatish orqali foydalanuvchi bilan interaktiv (interactive) aloqa vositasi.

Entry blokli kodlashda biz quyidagi ikkita blok (<img src="../.gitbook/assets/entry blocki.png" alt="" data-size="line"><img src="../.gitbook/assets/entry blocko.png" alt="" data-size="line">) yordamida kirish va chiqishni kodlagan edik.

Endi buni matnli kodlash orqali amalga oshiraylik. Kiritish/chiqish funksiyalarini biz avvalgi bo‘limda o‘rgangan **Entry** kutubxonasidagi ikki turdagi funksiyani (print, input) chaqirish orqali bajarish mumkin. Funksiya nomlari juda intuitiv bo‘lib, ularning vazifasi darhol tushunarli. Mazkur funksiyalar **Entry-Python** dasturida asl Python-dan bir oz farq bilan ishlaydi (_**asl Python-da bu funksiyalarni kutubxonani chaqirmasdan, to‘g‘ridan-to‘g‘ri ishlatish mumkin; bunday funksiyalar tilning o‘ziga xos bo‘lgan ichki funksiyalari bo‘lib, "ichki funksiyalar" deb ataladi**_). Ammo **Entry**da ular alohida kutubxona tarkibiga kiradi. Bu funksiyalarni qanday chaqirishni avvalgi bo‘limlarda ko‘rib chiqqanmiz: K**utubxonaNomi.FunksiyaNomi** ko‘rinishidagi sintaksis yordamida chaqiriladi. Shunday ekan, **Entry.print()** va **Entry.input()** funksiyalarini chaqirish mumkin. Biroq, funksiyaning to‘g‘ri ishlashi uchun chaqiruvchi tomonidan uzatilishi lozim bo‘lgan majburiy qiymatlar (parametrlar) qanday ekanini aniq bilish kerak.

Aslida, buni intuitiv tarzda taxmin qilish mumkin: **print** (chiqarish) funksiyasida foydalanuvchiga ko‘rsatmoqchi bo‘lgan xabarni uzatish kerak, **input** (kiritish) funksiyasida esa foydalanuvchidan olishni xohlagan ma’lumotni tushuntiruvchi xabarni uzatish kerak. Ushbu xabarlar odatda istalgan matn bo‘lib, kodlash dunyosida bu ma’lumot turi **string** (matn qatori) deb ataladi. Shu sababli, xabarni ifodalash uchun matnni _**" "(qo‘shtirnoqlar)**_ orasiga yozish kifoya. (Bittalik qo'shtirnoqdan(' ') foydalanish ham mumkin, lekin **Entry-Python** avtomatik ravishda uni ikkitalik qo'shtirnoqqa o‘zgartiradi.) Bundan tashqari, chiqarilmoqchi bo‘lgan xabarni bir nechta qismga ajratib, ularni birlashtirib chiqarish ham qiziqarli usuldir. Bir nechta matn qismlarini birlashtirish uchun foydalaniladigan operator **+** bo‘lib, u "matnlarni birlashtirish" degan mantiqiy ma’noni beradi.

Keling, hozirgacha nazariy jihatdan o'rgangan barcha narsalarni birlashtiramiz va foydalanuvchining yoshini kiritish va uni chiqaradigan matnli kodlash yordamida juda oddiy dasturni kodlaymiz.

{% tabs %}
{% tab title="Ijro natijasi" %}
<figure><img src="../.gitbook/assets/2we22 copy.png" alt="" width="375"><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Blokli kodlash" %}
<figure><img src="../.gitbook/assets/inout.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Entry-Python" %}
{% code lineNumbers="true" %}
```python
# (1)Entrybot's Python code

import Entry

def when_start():
    Entry.input("Iltimos, yoshingizni kiriting.")
    Entry.print((("Siz " + Entry.answer()) + " yoshdasiz."))
```
{% endcode %}
{% endtab %}
{% endtabs %}

Kodlarni tushunish qiyin emasmi? Biroz notanish bo‘lgan joy **Entry.answer()** deb yozilgan qismidir. Bu funksiya nima uchun kerak? _Aslida, bu funksiya faqat **Entry-Python** uchun zarur (haqiqiy Python-da foydalanuvchi kiritgan qiymatni dasturchi o‘zi aniqlagan o‘zgaruvchiga saqlab ishlatadi, shuning uchun bunday maqsadga mo‘ljallangan funksiya kerak emas). Ushbu funksiyaning vazifasi foydalanuvchi tomonidan kiritilgan qiymatni bilib olishdir. Bu yerda **Entry.print** funksiyasi ichida chiqarish xabarini tuzishda, foydalanuvchi kiritgan qiymatni olish va uni natija sifatida ko‘rsatishda foydalanilgan._

Ichki ishlash jarayonini biroz batafsilroq tushuntirsak, foydalanuvchi qandaydir qiymat kiritganida, bu qiymatni kodning boshqa qismida qayta ishlatish uchun uni qandaydir joyga vaqtinchalik saqlash kerak bo‘ladi (odatda bunday saqlash joyi **o‘zgaruvchi** deb ataladi). Keyin shu o‘zgaruvchi orqali kiritilgan qiymat kodning boshqa qismlarida ishlatiladi. Ammo bizning kodimizda o‘zimiz yaratgan birorta o‘zgaruvchi bo‘lmasada, kerakli natijani amalga oshirdi. Bu qanday sodir bo‘ldi? Haqiqatda, **Entry** ichki tizimida foydalanuvchi kiritgan qiymat vaqtinchalik yashirin o‘zgaruvchida saqlanadi. Bizga esa faqat ushbu qiymatni o‘qib olish uchun **answer()** funksiyasi taqdim etiladi. Yuqorida aytib o‘tilganidek, haqiqiy Python dasturlashida bunday usul ishlatilmaydi. Ammo **Entry** blokli kodlashda foydalanuvchilar uchun maksimal qulaylikni ta'minlash maqsadida bu zarurat tug‘ilgan. **Entry-Python** ham blokli kodlashni to‘liq davom ettiruvchi va foydalanuvchilarni matnli kodlashga o‘tishga o‘rgatuvchi oraliq ko‘prik sifatida xizmat qiladi. Shuning uchun ham, **Entry-Python** Python-ni mukammal o‘rganish vositasi emas, balki blokli kodlashdan matnli kodlashga o‘tishda yordam beruvchi vosita ekanligini ushbu misoldan ham bilib olishimiz mumkin.
