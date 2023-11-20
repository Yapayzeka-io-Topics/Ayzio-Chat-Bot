
[ayzio.org](https://www.ayzio.org) tarafından ❤️ ile oluşturuldu.

## Açıklama

- Bu React uygulaması [create-react-app](https://create-react-app.dev/) kullanılarak oluşturulmuştur.
- [Tailwind CSS](https://tailwindcss.com/) kullanmaktadır.
- Uygulama JavaScript dilinde oluşturulmuştur.

## Ön Koşullar

- [git](https://git-scm.com/) - v2.13 veya üstü
- [NodeJS](https://nodejs.org/en/) - v16 veya üstü
- [npm](https://www.npmjs.com/) - v6 veya üstü

## Geliştirme Ortamında Çalıştırma

1. `cd UYGULAMA_DIZINI`
2. `npm install`
3. `npm start`

## .env Dosyası

Bu dosya çeşitli ortam değişkenlerini içermektedir ve bunları yapılandırabilirsiniz.

# Storybook'u Çalıştırma

Ortak bileşenleri algıladık ve olası varyasyonlarını oluşturduk. Storybook'u entegre ederek oluşturulan ortak bileşenlerin belgelerini kontrol etmek için lütfen aşağıdaki adımları izleyin.

## Kurulum ve Başlatma

npx storybook init


## Storybook'u Çalıştırma

npm run storybook


## Klasör Yapısı

.
├── package.json
├── postcss.config.js
├── public
│   ├── assets
│   │   └── images --------- Tüm Proje Görselleri
│   ├── favicon.ico
│   ├── index.html
│   ├── manifest.json
│   └── robots.txt
├── README.md
├── src
│   ├── App.jsx
│   ├── assets
│   │   └── fonts ---------- Proje Fontları
│   ├── components --------- UI ve Algılanan Ortak Bileşenler
│   ├── constants ---------- Proje sabitleri, örneğin: string sabitleri
│   ├── hooks -------------- Yardımcı Hooks
│   ├── index.jsx
│   ├── pages -------------- Tüm rota sayfaları
│   ├── Routes.jsx ---------- Yönlendirme
│   ├── styles
│   │   ├── index.css ------ Diğer Global Stiller
│   │   └── tailwind.css --- Varsayılan Tailwind modülleri
│   └── util
│       └── index.jsx ------- Yardımcı yardımcılar
└── tailwind.config.js ----- Tüm tema yapılandırması, renkler, fontlar vb.


less
Copy code

Projeyi derlemek için **bu dosyaların kesin dosya adlarıyla mevcut olması gerekir**:

- `public/index.html` sayfa şablonudur;
- `src/index.jsx` JavaScript giriş noktasıdır.

src içinde alt dizinler oluşturabilirsiniz.

## Kullanılabilir Komut Dosyaları

Projedeki dizinde aşağıdaki komutları çalıştırabilirsiniz:

### `npm start`

Uygulamayı geliştirme modunda çalıştırır.<br>
Tarayıcıda görmek için [http://localhost:3000](http://localhost:3000) adresini açın.

### `npm test`

Etkileşimli izleme modunda test çalıştırır.<br>

### `npm run build`

Uygulamayı üretim için `build` klasörüne derler.<br>

### `npm run eject`

**Not: Bu tek yönlü bir işlemdir. Bir kez `eject` yaparsanız, geri dönemezsiniz!**

Eğer derleme aracı ve yapılandırma seçimlerinizden memnun değilseniz, istediğiniz zaman `eject` yapabilirsiniz.

## Bağımlılık Yüklemek

Herhangi bir bağımlılığı (örneğin, React Router) `npm` ile yükleyebilirsiniz:

```sh
npm install --save react-router
Alternatif olarak yarn kullanabilirsiniz:

sh
Copy code
yarn add react-router
Lisans
MIT Lisansı

Telif Hakkı (c) 2023 Ayzio.org

Bu yazılımın ve ilişkili belge dosyalarının ( "Yazılım" ) bir kopyasını edinen herkese, yazılımı sınırlama olmaksızın kullanma, kopyalama, değiştirme, birleştirme, yayınlama, dağıtma, alt lisanslama ve/veya yazılımın kopyalarını satma izni verilmiştir ve yazılımı sağlayan kişilere veya kuruluşlara aşağıdaki şartlar altında yapmalarına izin verilir:

Yukarıdaki telif hakkı bildirimi ve bu izin bildirimi, yazılımın tüm kopyalarına veya önemli bir kısmına eklenmelidir.

YAZILIM "AS IS" TEMİNATIYLA, BELİRLİ BİR AMAÇA UYGUNLUK VEYA İHLAL ETMEME GARANTİSİ İÇİNDE OLMADAN SAĞLANMIŞTIR. HERHANGİ BİR DURUMDA YAZARLAR VEYA TELİF HAKKI SAHİPLERİ, SÖZLEŞME, HAKKANİYET VEYA DİĞER GİBİ, İHLAL, HASAR VEYA DİĞER DURUMLARDA, YAZILIMIN KULLANIMINDAN, KULLANIL...
