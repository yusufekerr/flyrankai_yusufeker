# Proje Kuralları — Frontend AI Playground

Bu dosya, projede tutarlı kod kalitesi ve geliştirme pratikleri sağlamak için Cursor AI ve ekip üyelerine yönelik kuralları tanımlar.

## Genel İlkeler

- Kod okunabilir, sade ve bakımı kolay olmalıdır.
- Gereksiz soyutlama ve erken optimizasyondan kaçınılır.
- Mevcut dosya yapısı ve kod stiline uyulur; yeni desenler yalnızca gerçekten gerekli olduğunda eklenir.
- Commit mesajları [Conventional Commits](https://www.conventionalcommits.org/) formatında yazılır.

## TypeScript

- `any` kullanımından kaçınılır; gerekirse `unknown` tercih edilir.
- Tip tanımları mümkün olduğunca açık ve dar kapsamlı tutulur.
- Paylaşılan tipler `src/types/` altında toplanır.
- Interface ve type alias seçiminde proje içindeki mevcut kullanım takip edilir.

## React

- Yalnızca fonksiyonel bileşenler kullanılır.
- Tekrar kullanılabilir mantık `src/hooks/` altında custom hook olarak ayrılır.
- Bileşenler tek sorumluluk ilkesine uygun, küçük ve odaklı tutulur.
- Prop tipleri bileşenle birlikte tanımlanır veya ayrı bir tip dosyasına taşınır.
- Side effect'ler `useEffect` içinde açık bağımlılık dizileriyle yönetilir.

## Dosya ve Klasör Yapısı

```
src/
├── assets/       # Statik dosyalar (svg, img)
├── components/   # Yeniden kullanılabilir UI bileşenleri
├── hooks/        # Custom React hook'ları
├── pages/        # Sayfa düzeyinde bileşenler
├── types/        # Paylaşılan TypeScript tipleri
├── utils/        # Saf yardımcı fonksiyonlar
├── App.tsx
├── main.tsx
└── index.css
```

- Bileşen dosyaları PascalCase (`Button.tsx`, `UserCard.tsx`) ile adlandırılır.
- Hook dosyaları `use` önekiyle camelCase (`useAuth.ts`) adlandırılır.
- Yardımcı fonksiyonlar camelCase (`formatDate.ts`) adlandırılır.

## Stil ve CSS

- Global stiller `src/index.css` içinde tutulur.
- Bileşene özel stiller mümkünse bileşen dosyasıyla birlikte konumlandırılır.
- Sınıf adları anlamlı ve tutarlı olmalıdır.

## API ve Veri Yönetimi

- API çağrıları `src/services/` veya `src/api/` altında toplanır.
- Fetch/HTTP hataları kullanıcıya anlamlı mesajlarla iletilir.
- Yükleme ve hata durumları UI'da açıkça gösterilir.

## Lint ve Kalite

- Commit öncesi `npm run lint` çalıştırılması önerilir.
- Oxlint uyarıları gerekçesiz biçimde susturulmaz (`eslint-disable` benzeri yorumlar).
- Ölü kod, kullanılmayan import ve gereksiz console.log bırakılmaz.

## Commit Mesajları

Format: `<type>(<scope>): <açıklama>`

| Type       | Kullanım                          |
| ---------- | --------------------------------- |
| `feat`     | Yeni özellik                      |
| `fix`      | Hata düzeltmesi                   |
| `docs`     | Dokümantasyon                     |
| `style`    | Biçimlendirme (mantık değişmez)   |
| `refactor` | Davranış değiştirmeyen yeniden yapılandırma |
| `test`     | Test ekleme veya güncelleme       |
| `chore`    | Araç, bağımlılık, yapılandırma    |

Örnekler:

```
feat(auth): add login form validation
fix(api): handle 404 response in user fetch
docs: update README with deployment steps
```

## AI Asistan Kullanımı

- Yapılan değişiklikler minimal kapsamda tutulur; istenmeyen dosyalar değiştirilmez.
- Yeni bağımlılık eklenmeden önce mevcut çözümler değerlendirilir.
- Test, dokümantasyon veya refactor yalnızca istendiğinde veya anlamlı katkı sağladığında eklenir.
