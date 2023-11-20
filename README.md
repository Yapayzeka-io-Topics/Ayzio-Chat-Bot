
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

## Storybook'u Çalıştırma

Storybook'u çalıştırmak için aşağıdaki adımları takip edebilirsiniz:

1. **Proje Dizinine Git:**
    ```bash
    cd Proje_Dizini
    ```

2. **Bağımlılıkları Yükle:**
    ```bash
    npm install
    ```

3. **Storybook'u Başlat:**
    ```bash
    npm run storybook
    ```

## Klasör Yapısı

import java.util.ArrayList;
import java.util.List;

class FileOrFolder {
    private String name;
    private boolean isFile;
    private List<FileOrFolder> children;

    public FileOrFolder(String name, boolean isFile) {
        this.name = name;
        this.isFile = isFile;
        this.children = new ArrayList<>();
    }

    public void addChild(FileOrFolder child) {
        this.children.add(child);
    }

    public void display(String indent) {
        System.out.println(indent + (isFile ? "├── " : "└── ") + name);
        for (int i = 0; i < children.size(); i++) {
            if (i < children.size() - 1) {
                children.get(i).display(indent + (isFile ? "│   " : "    "));
            } else {
                children.get(i).display(indent + (isFile ? "    " : "    "));
            }
        }
    }
}

public class FolderStructure {
    public static void main(String[] args) {
        // Klasör yapısını oluştur
        FileOrFolder root = new FileOrFolder("Proje", false);

        FileOrFolder publicFolder = new FileOrFolder("public", false);
        FileOrFolder assetsFolder = new FileOrFolder("assets", false);
        FileOrFolder imagesFolder = new FileOrFolder("images", false);

        FileOrFolder srcFolder = new FileOrFolder("src", false);
        FileOrFolder assetsSrcFolder = new FileOrFolder("assets", false);
        FileOrFolder fontsFolder = new FileOrFolder("fonts", false);

        FileOrFolder stylesFolder = new FileOrFolder("styles", false);

        FileOrFolder utilFolder = new FileOrFolder("util", false);

        root.addChild(publicFolder);
        publicFolder.addChild(assetsFolder);
        assetsFolder.addChild(imagesFolder);

        root.addChild(srcFolder);
        srcFolder.addChild(assetsSrcFolder);
        assetsSrcFolder.addChild(fontsFolder);

        srcFolder.addChild(stylesFolder);

        srcFolder.addChild(utilFolder);

        // Klasör yapısını göster
        root.display("");
    }
}

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
