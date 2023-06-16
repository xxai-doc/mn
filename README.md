<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.art

Вэбсайт кодын нэг хэсэг нь нээлттэй эх сурвалж бөгөөд орчуулгыг оновчтой болгоход тавтай морилно уу.

## урд талын код

* [урд талын код](https://github.com/xxai-art/web)
* [Бүхэл бүтэн сайтад зориулсан хэлний багц](https://github.com/xxai-art/web/tree/main/i18n)
* [Нэвтрэх модулиудын хэлний багц](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Вэб сайтын олон хэл дээрх баримтжуулалт](https://github.com/xxai-doc)

Урд талын програмчлалын хэл нь [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) бөгөөд кофекриптийн синтакс дээр суурилсан зарим функцийг нэмдэг, [./coffee_plus.md -г](./coffee_plus.md) үзнэ үү.

## Вэбсайт, баримт бичгийг олон улсын болгох

Дараах 3 төсөл дээр тулгуурлана

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Дагавар нь `.mdt` , та `<+ ./coffee_plus/import.js>` төстэй синтаксийг ашиглан гадаад файлуудыг дурдаж, `.md` дагавараар тэмдэглэгээ үүсгэж болно.

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  Markdown орчуулга нь код болон холбоосыг орчуулахгүй бөгөөд орчуулсан өгүүлбэрийг кэш болгоно. Хэрэв орчуулга өөрчлөгдсөн боловч эх текст өөрчлөгдөөгүй бол түүнийг дахин гүйцэтгэх нь орчуулгын өөрчлөлтийг дарж бичихгүй.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  `yaml` үүсгэсэн вэбсайтуудыг орчуулах хэлний файлууд.
