<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Сан руу орсны дараа эхлээд nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) суулгаж, дараа нь `direnv allow` програмуудыг суулгахыг зөвлөж байна ( [.envrc нь](https://github.com/xxai-art/doc/blob/main/.envrc) лавлах руу орсны дараа автоматаар ажиллана).

Утга нь: Хятад, Япон, Солонгос, Англи, бусад бүх хэл рүү англи орчуулга. Хэрэв та зөвхөн хятад, англи хэлийг дэмжихийг хүсвэл `zh: en` бичээд л болно.

Утга нь: Хятад, Япон, Солонгос, Англи, бусад бүх хэл рүү англи орчуулга. Хэрэв та зөвхөн хятад, англи хэлийг дэмжихийг хүсвэл `zh: en` бичээд л болно.

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

  Markdown орчуулга нь код болон холбоосыг орчуулахгүй бөгөөд орчуулсан өгүүлбэрийг кэш болгоно. Хэрэв орчуулга өөрчлөгдсөн боловч эх бичвэр өөрчлөгдөөгүй бол түүнийг дахин гүйцэтгэх нь орчуулгын өөрчлөлтийг дарж бичихгүй.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  `yaml` үүсгэсэн вэбсайтуудыг орчуулах хэлний файлууд.

### Баримт бичгийн орчуулгыг автоматжуулах заавар

[xxai-art/doc](https://github.com/xxai-art/doc) кодын агуулахыг үзнэ үү

Сан руу орсны дараа эхлээд nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) суулгаж, дараа нь `direnv allow` програмуудыг суулгахыг зөвлөж байна ( [.envrc нь](https://github.com/xxai-art/doc/blob/main/.envrc) лавлах руу орсны дараа автоматаар ажиллана).

Олон зуун хэл рүү хөрвүүлсэн том кодын сангаас зайлсхийхийн тулд би хэл бүрт тусдаа кодын бааз үүсгэж, кодын санг хадгалах байгууллагыг бий болгосон.

`GITHUB_ACCESS_TOKEN` орчны хувьсагчийг тохируулаад [create.github.coffee-г](https://github.com/xxai-art/doc/blob/main/create.github.coffee) ажиллуулснаар автоматаар кодын агуулах үүсгэнэ.

Мэдээжийн хэрэг та үүнийг кодын баазад хийж болно.

Орчуулгын скриптийн лавлагаа [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Скрипт кодыг дараах байдлаар тайлбарлав.

[bunx](https://bun.sh/docs/cli/bunx) нь npx-ийн орлуулалт бөгөөд илүү хурдан байдаг. Мэдээжийн хэрэг, хэрэв танд bun суулгаагүй бол оронд нь `npx` ашиглаж болно.

`bunx mdt zh` `.mdt` г zh лавлах дотор `.md` гэж дүрсэлдэг бол доорх холбоос бүхий 2 файлыг үзнэ үү.

* [coffee_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [coffee_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` нь орчуулгын үндсэн код юм (хэрэв танд зөвхөн `nodejs` суулгасан боловч `bun` болон `direnv` суулгаагүй бол та мөн орчуулахын тулд `npx i18n` ажиллуулж болно).

Энэ нь [i18n.yml-г](https://github.com/xxai-art/doc/blob/main/i18n.yml) задлах бөгөөд энэ баримт бичигт `i18n.yml` ийн тохиргоо дараах байдалтай байна:

```
en:
zh: ja ko en
```

Утга нь: Хятад, Япон, Солонгос, Англи, бусад бүх хэл рүү англи орчуулга. Хэрэв та зөвхөн хятад, англи хэлийг дэмжихийг хүсвэл `zh: en` бичээд л болно.

Сүүлийнх нь [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) бөгөөд энэ нь хэл бүрийн `README.md` ийн үндсэн гарчиг болон эхний хадмал гарчиг хоорондын агуулгыг задлан гаргаж, `README.md` оруулгыг үүсгэдэг. Код нь маш энгийн тул та өөрөө харж болно.

Google API-г үнэгүй орчуулахад ашигладаг. Хэрэв та Google-д нэвтэрч чадахгүй бол дараах прокси тохиргоог хийж тохируулна уу.

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Орчуулгын скрипт нь `.i18n` директорт орчуулагдсан кэш үүсгэх бөгөөд дахин орчуулахаас зайлсхийхийн тулд үүнийг `git status` шалгаад кодын хадгалах санд нэмнэ үү.

Кэшийг шинэчлэхийн тулд орчуулгыг өөрчлөх бүрдээ `bunx i18n` г ажиллуулна уу.

Хэрэв эх текст болон орчуулгыг нэгэн зэрэг өөрчилвөл кэш андуурч, өөрчлөхийг хүсвэл зөвхөн нэгийг нь өөрчилж, дараа нь `bunx i18n` програмыг ажиллуулж кэшийг шинэчилнэ үү.
