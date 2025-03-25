# 4.1 Ketma-ket/Parallel bajarish (Serial/Parallel)

**Ketma-ket/parallel bajarish tushunchasi aslida dasturlash paradigmasi emas. Oddiy qilib aytganda, bu bir nechta vazifalarni ketma-ket yoki bir vaqtning o'zida ularni bajarish tartibida farqdir.**

Ketma-ket bajarish (Serial processing) — kod qatorlarini birin-ketin bajarishni anglatadi. Bu tushuncha kompyutersiz (unplugged) kodlash ta'limida ham eng asosiy mavzu bo‘lib, aslida hammamiz yaxshi biladigan oddiy tushuncha, shuning uchun alohida tushuntirishga hojat yo‘q. Paralel bajarish (Parallel processing) esa kompyuter muhandisligi nazariyasida murakkabroq tushuncha bo‘lib, yangi boshlovchilar uchun tushunish qiyin bo‘lishi mumkin. Bundan tashqari, Entry yoki Python kabi platformalarda bunday darajadagi parallel bajarish qo‘llab-quvvatlanmaydi, shuning uchun faqat asosiy tushunchani bilib o‘tish yetarli. **Parallel bajarish bir nechta vazifani bir vaqtning o‘zida bajarish** usuli sifatida tushuntiriladi. Bunda haqiqiy vazifalar butunlay mustaqil holda bajariladimi (paralellik, Parallelism), yoki vazifalar go‘yoki bir vaqtda bajarilayotgandek ko‘rinish hosil qiluvchi texnika (sinxronlik, Concurrency) yordamida bajariladimi, bu ikki tushunchani farqlash muhim. Entry va Python platformalari ikkinchi usulga — sinxronlikka tayanadi.

Entry-Python platformasida sinxronlik (concurrency) bilan bog‘liq dasturlash texnikalari (oqimlar, ko‘p -jarayonlik va boshqalar) qo‘llab-quvvatlanmagani sababli, bu usullardan foydalanib kod yozishni yoki sinxronlikka oid dasturlash usullarini o‘rganishni imkonsiz qiladi. Kitobning boshida ham ta'kidlanganidek, bu Entry-Python platformasining cheklovidir. Shu bilan birga, Entry-Python dastlab blokli kodlashdan birinchi matnli kodlashga o‘tganlar uchun mo‘ljallangan bo‘lib, murakkab darajadagi o‘rganish maqsad qilinmagan. Shuning uchun, asosiy tushunchalarni o‘zlashtirib, texnik tafsilotlarga chuqur kirmasdan o‘tishning o‘zi kifoya. Haqiqatan ham, bu darajadagi tushunchalar ham o‘z ahamiyatiga ega ekanligini bilish foydali bo‘ladi.

Entry blokli kodlashida, quyidagi misolda ko‘rganingizdek, biz allaqachon ko‘p bor paralel bajarishni kodlab ko‘rganmiz.

{% tabs %}
{% tab title="Ijro natijasi" %}
<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Blokli kodlash" %}
<figure><img src="../.gitbook/assets/sr (1).png" alt="" width="375"><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Entry-Python" %}
{% code lineNumbers="true" %}
```python
# Changyutgich robot(1)'s Python code

import Entry

def when_start():
    Entry.start_drawing()
    Entry.set_brush_color_to("#FFFFFF")
    Entry.set_brush_size(50)

def when_start():
    while True:
        Entry.move_to_direction(10)
        if Entry.is_touched("edge"):
            Entry.move_to_direction(-15)
            Entry.add_rotation(133)
```
{% endcode %}
{% endtab %}
{% endtabs %}

“Boshlash tugmasini bosganda” deb nomlangan blokni bir obyektda bir necha marta ishlatib, mustaqil ko‘rinadigan vazifalarni go‘yoki bir vaqtning o‘zida bajarilayotgandek kodlagan tajribamiz bor edi. Bu orqali biz turli dasturlashning asosiy tushunchalaridan foydalanib kelganmiz, buni o‘zimiz sezmagan holda bajargan bo‘lsak ham.

Shu sababli, Entry-Python da paralel bajarish blokli kodlashda qilgan ishlarimizdan unchalik farq qilmaydi. Faqat yuqoridagi misolda ko‘rsatilganidek, **when\_start** funksiyasini bir necha marta ishlatish mumkin. Foydalanuvchi dastur ishga tushishi uchun “Boshlash” tugmasini bosganda, har bir **when\_start** funksiyasi bir vaqtning o‘zida chaqiriladi. Shu tarzda, har bir funksiyada bajarilishi kerak bo‘lgan vazifalarni mustaqil ravishda tasvirlab, ularni go‘yoki bir vaqtda bajarilayotgandek ko‘rinish hosil qilish mumkin. Bu usulni kodlashda va dasturda samarali foydalanish kifoya qiladi.
