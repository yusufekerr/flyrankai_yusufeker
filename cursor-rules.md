# Proje Kuralları – Frontend AI Playground

Bu dosya, proje boyunca Cursor'ın nasıl çalışacağını, kodlama standartlarını, commit kurallarını ve yapay zekâ destekli geliştirme yöntemlerini tanımlar.

---

## 1) Teknoloji Yığını

- React + TypeScript
- Vite geliştirme ortamı
- Modern, bileşen tabanlı frontend mimarisi
- Yapay zekâ destekli geliştirme (Cursor / Claude)

---

## 2) Dosya Yapısı Kuralları

- `src/components/` → Tekil UI bileşenleri
- `src/pages/` → Sayfa yapıları
- `src/utils/` → Yardımcı fonksiyonlar
- `public/` → Statik dosyalar
- Her bileşen kendi klasöründe olmalı (component-name/index.tsx + component-name.css)

---

## 3) Kodlama Standartları

- TypeScript zorunlu
- Fonksiyon ve bileşen isimleri İngilizce olmalı
- Dosya isimleri kebab-case
- Bileşen isimleri PascalCase
- Gereksiz yorum satırı kullanılmamalı
- UI sade, responsive ve minimal olmalı

---

## 4) Commit Kuralları (Conventional Commits)

Commit mesajları şu formatta olmalıdır:

```
<type>: <açıklama>
```

### Kullanılabilir type'lar:

- **feat:** yeni özellik
- **fix:** hata düzeltme
- **docs:** dokümantasyon değişiklikleri
- **chore:** yapılandırma, bağımlılık, ayar
- **refactor:** davranışı değiştirmeyen kod iyileştirmesi
- **style:** format, boşluk, noktalama
- **test:** test ekleme/düzeltme

### Örnekler:

```
feat: add AI prompt input component
docs: update README with setup instructions
chore: configure eslint and prettier
```

---

## 5) Yapay Zekâ Kullanım Kuralları

Cursor'dan şu konularda yardım istenir:

- Kod oluşturma
- Kod iyileştirme
- Dosya yapısı düzenleme
- Dokümantasyon yazma
- Refactor önerileri
- Hata analizi

Cursor'dan **şu konularda yardım istenmez**:

- Proje amacı dışında dosya oluşturma
- Gereksiz karmaşık mimari önerileri
- Drag-and-drop tarzı otomatik UI üretimi

---

## 6) Prompt Yazım Kuralları

Cursor'a verilen komutlar:

- Net
- Adım adım
- Gereksiz açıklama içermeyen
- Teknik olarak yönlendirilmiş olmalıdır

### Örnek:

```
Bu bileşeni TypeScript ile oluştur. Props olarak promptText alacak. Submit edildiğinde handlePrompt fonksiyonunu çalıştıracak.
```

---

## 7) Hedef

Bu proje, yapay zekâ destekli frontend geliştirme becerilerini göstermek için oluşturulmuştur. Amaç:

- Temiz kod
- Düzenli commit geçmişi
- AI ile iş birliği kanıtı
- Profesyonel proje yapısı
