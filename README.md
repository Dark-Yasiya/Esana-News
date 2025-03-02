<p align="center">
  <a href="" rel="noopener">
 <img width=100px height=100px src="https://www.helakuru.lk/assets/images/helakuru-logo1.png" alt="Esana"></a>
</p>

<h2 align="center">Esana News Scrap</h2>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/Dark-Yasiya/Esana-News.svg)](https://github.com/Dark-Yasiya/Esana-News/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/Dark-Yasiya/Esana-News.svg)](https://github.com/Dark-Yasiya/Esana-News/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> The unofficial Scrap [Esana]
    <br> 
</p>

## 📝 Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Usage](#usage)
- [Authors](#authors)

## 🧐 About <a name = "about"></a>

The unofficial Scrap [Esana]

## 🏁 Getting Started <a name = "getting_started"></a>

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Installing


```sh
yarn add @dark-yasiya/esana-news
```

or

```sh
npm i @dark-yasiya/esana-news
```

## 🎈 Usage <a name="usage"></a>

```ts
const Esana = require('@dark-yasiya/esana-news');

var esana = new Esana();
```
## Get all news
```ts
await esana.newsList();
```


```ts
{
  status: true,
  creator: 'Dark-Yasiya',
  data: [
    {
      title: 'මොරටු රන් මහා සටන ජය පරාජයෙන් තොරව අවසන් වෙයි',
      image: 'https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/battle-golds-2025.jpg',
      ago: '1 Hour ago',
      id: '107952'
    },
    {
      title: 'ආනන්ද නාලන්ද සුලෝහිත සංග්‍රාමය ජය පරාජයෙන් තොරව අවසන් වෙයි',
      image: 'https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/battle-of-maroons-2025.jpg',
      ago: '1 Hour ago',
      id: '107951'
    },
    {
      title: 'විශේෂ දළදා ප්‍රදර්ශනය අප්‍රේල් 18 වනදා ඇරඹෙයි',
      image: 'https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/dalada[1].jpg',
      ago: '1 Hour ago',
      id: '107950'
    },
    {
      title: 'කීත් නොයාර් පැහැරගැනීමේ සිද්ධියට හිටපු බුද්ධි අංශ නිලධාරි දෙදෙනෙක් අත්අඩංගුවට',
      image: 'https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/arrested2[1].jpg',
      ago: '4 Hours ago',
      id: '107949'
    },
   ...
  ]
}
```
## Get latest news

```ts
await esana.latestNews();
```
```ts
{
  status: true,
  creator: 'Dark-asiya',
  data: {
    title: 'මොරටු රන් මහා සටන ජය පරාජයෙන් තොරව අවසන් වෙයි',
    image: ' https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/battle-golds-2025.jpg',
    ago: '1 Hour ago',
    desc: '\n' +
      'මොරටුව වේල්ස් කුමර විද්‍යාලය සහ ශාන්ත සෙබස්තියන් විද්‍යාලය අතර පැවැත්වෙන 75 වැනි ‘මොරටු රන් මහා සටන’ වාර්ෂික ක්‍රිකට් තරගය ජය පරාජයෙන් තොරව අවසන් වුණා.\n' + 
      'තරගයේ කාසියේ වාසිය දිනාගත් ශාන්ත සෙබස්තියන් විද්‍යාලය පළමුවෙන් පන්දුවට පහරදීමට මොරටුව වේල්ස් කුමර විද්‍යාලයට ආරාධනා කළ අතර ඔවුන් සිය පළමු ඉනිම සඳහා සියලු දෙන
ා දැවී ලකුණු 161 ක් ලබාගත්තා.\n' +
      'ඉන් අනතුරුව සිය පළමු ඉනිම සඳහා පන්දුවට පහරදීමට පැමිණි ශාන්ත සෙබස්තියන් විද්‍යාලය සියලු දෙනා දැවී ලකුණු 208 ක් ලබා ගත්තා.\n' +
      'යළි දෙවන ඉනිම සඳහා පන්දුවට පහරදුන් මොරටුව වේල්ස් කුමර විද්‍යාලය කඩුලු 6 ක් දැවී ලකුණු 157 ක් ලබාගත් අතර ඒ අනුව තරගය ජය පරාජයෙන් තොරව අවසන් කිරීමට තීරණය කර ඇත
ි බවයි වැඩිදුරටත් සඳහන් වෙන්නේ.\n' +
      '\n'
  }
}
```
## Get news info for id

```ts
let id = "107951";
await esana.newsInfo(id);
```
```ts
{
  status: true,
  creator: 'Dark-Yasiya',
  data: {
    title: 'ආනන්ද නාලන්ද සුලෝහිත සංග්‍රාමය ජය පරාජයෙන් තොරව අවසන් වෙයි',
    image: ' https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/battle-of-maroons-2025.jpg',
    ago: '1 Hour ago',
    desc: '\n' +
      'ආනන්ද විද්‍යාලය සහ නාලන්දා විද්‍යාලය අතර 95 වන සුලෝහිත සංග්‍රාමය ජය පරාජයෙන් තොරව අවසන් වී තිබෙනවා.\n' +
      'ආනන්ද විද්‍යාලය පළමු ඉනිම සඳහා කඩුලු 6ක් දැවී ලකුණු 324ක් ලබා ගත් අතර ඉන් පසුව ඉනිම අත්හිටුවා පන්දුවට පහරදීමට නාලන්දා විද්‍යාලයට ආරධනා කර තිබුණා.\n' +       
      'ඒ අනුව නාලන්දා විද්‍යාලය පළමු ඉනිම සඳහා කඩුලු 6ක් දැවී ලකුණු 325ක් ලබා ගනිමින් ඉනිම අත්හිටුවා නැවතත් පන්දුවට පහර දීමට ආනන්ද විද්‍යාලය අවස්ථාව ලබාදුන්නා.\n' +
      'සිය දෙවනි ඉනිම සඳහා පන්දුවට පහර දීමට පිටියට පිවිසි ආනන්ද විද්‍යාලය දිනය නිමාවන විට කඩුලු 1ක් දැවී ලකුණු 27ක් ‍රැස් කර ගැනීමට සමත් වූ අතර ඒ අනුව තරගය ජය පරාජය
ෙන් තොරව අවසන් වුණා.\n' +
      '\n'
  }
}
```
## ✍️ Authors <a name = "authors"></a>

- [@Dark-Yasiya](https://github.com/Dark-Yasiya) - scraped project author

See also the list of [contributors](https://github.com/Dark-Yasiya/Esana-News/contributors) who participated in this project.
