# PCAT – Fotoğraf Yükleme Uygulaması

Bu proje, Node.js ve Express.js kullanılarak geliştirilen basit bir fotoğraf yükleme uygulamasıdır. Amaç, backend geliştirme sürecinde sık kullanılan araç ve kavramları pratik bir proje üzerinden öğrenmektir.

## 🚀 Özellikler

- **Fotoğraf Yükleme:** Kullanıcılar sisteme kendi fotoğraflarını yükleyebilir.
- **CRUD İşlemleri:** Fotoğraf ekleme (Create), detaylarını görüntüleme/listeleme (Read), güncelleme (Update) ve silme (Delete) işlemleri sorunsuz bir şekilde çalışır.
- **Dinamik Sayfalar:** İçerikler EJS template engine kullanılarak dinamik olarak render edilmektedir.
- **MVC Mimarisi:** Proje yapısı Model, View ve Controller prensiplerine göre modüler bir düzende inşa edilmiştir.

## 🛠️ Kullanılan Teknolojiler

- **Backend:** Node.js, Express.js
- **Veritabanı:** MongoDB, Mongoose
- **Şablon Motoru (Template Engine):** EJS
- **Dosya Yükleme:** express-fileupload
- **Araçlar ve Middleware'ler:** dotenv (Çevre değişkenleri için), method-override (PUT ve DELETE HTTP istekleri için)
- **Geliştirme Araçları:** Nodemon, Prettier

## 📂 Klasör Yapısı

```text
PCAT/
├── controllers/       # Route işlemlerini gerçekleştiren kontroller (photoController)
├── models/            # Veritabanı şemalarının bulunduğu dosyalar (Photo modeli)
├── public/            # İstemci tarafında kullanılan statik dosyalar (CSS, JS)
├── views/             # Arayüz tasarımına ait EJS şablonları (index, about, add, edit vb.)
├── uploads/           # Yüklenen fotoğrafların saklandığı yerel dizin
├── app.js             # Uygulamanın çalışmaya başladığı ana dosya
├── .env               # Hassas ortam değişkenleri (Port, DB URI)
└── package.json       # Projenin paket bilgileri ve NPM script'leri
```

## ⚙️ Kurulum ve Çalıştırma

Projeyi yerel ortamınızda çalıştırmak için aşağıdaki adımları sırasıyla izleyebilirsiniz:

### 1. Projeyi Klonlayın

```bash
git clone https://github.com/Enesyldrm00/PCAT.git
cd PCAT
```

### 2. Gerekli Paketleri Yükleyin

```bash
npm install
```

### 3. Çevre Değişkenlerini (Environment Variables) Ayarlayın

Projenin kök dizininde bir `.env` dosyası oluşturun ve MongoDB bağlantı metniniz ile port numaranızı belirleyin. Örnek:

```env
PORT=5000
MONGO_URI=mongodb+srv://<kullanici_adiniz>:<sifreniz>@cluster0...mongodb.net/<veritabani_adi>?retryWrites=true&w=majority
```

### 4. Projeyi Başlatın

```bash
npm start
```
Uygulamanın başarıyla başlatıldığını terminalde göreceğiniz `Server: 5000` ve `DB connected` mesajlarından doğrulayabilirsiniz. Ardından tarayıcınız üzerinden şu linki açın: `http://localhost:5000`

## 👨‍💻 Yazar
**Muhammed Enes Yıldırım**
