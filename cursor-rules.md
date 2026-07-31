# Project Rules – Frontend AI Playground

This document defines how Cursor should work throughout the project, including coding standards, commit conventions, and AI-assisted development practices.

---

## 1) Tech Stack

- React + TypeScript
- Vite development environment
- Modern, component-based frontend architecture
- AI-assisted development (Cursor / Claude)

---

## 2) File Structure Rules

- `src/components/` → Individual UI components
- `src/pages/` → Page layouts
- `src/utils/` → Helper functions
- `public/` → Static assets
- Each component must live in its own folder (`component-name/index.tsx` + `component-name.css`)

---

## 3) Coding Standards

- TypeScript is required
- Function and component names must be in English
- File names use kebab-case
- Component names use PascalCase
- Avoid unnecessary comments
- UI should be clean, responsive, and minimal

---

## 4) Commit Rules (Conventional Commits)

Commit messages must follow this format:

```
<type>: <description>
```

### Available types:

- **feat:** new feature
- **fix:** bug fix
- **docs:** documentation changes
- **chore:** configuration, dependencies, setup
- **refactor:** code improvement without behavior change
- **style:** formatting, spacing, punctuation
- **test:** add or update tests

### Examples:

```
feat: add AI prompt input component
docs: update README with setup instructions
chore: configure eslint and prettier
```

---

## 5) AI Usage Rules

Ask Cursor for help with:

- Code generation
- Code improvement
- File structure organization
- Documentation
- Refactor suggestions
- Error analysis

Do **not** ask Cursor for:

- Creating files outside the project scope
- Unnecessarily complex architecture suggestions
- Drag-and-drop style automatic UI generation

---

## 6) Prompt Writing Rules

Commands given to Cursor should be:

- Clear
- Step-by-step
- Free of unnecessary explanation
- Technically directed

### Example:

```
Create this component in TypeScript. It should accept promptText as a prop. On submit, it should call the handlePrompt function.
```

---

## 7) Goal

This project was created to demonstrate AI-assisted frontend development skills. The aim is:

- Clean code
- A well-organized commit history
- Evidence of collaboration with AI
- A professional project structure

---

# Proje Kuralları – Frontend AI Playground (Türkçe)

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
