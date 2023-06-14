# spotify - grup oturumu

bu web site yazılımı, arkadaşlarınız ile spotify üzerinden grup oturumu ile müzik dinlemenizi sağlar. oluşturulan bir grup oturumunda; tüm katılımcılar sıraya şarkı ekleyebilir, kaldırabilir veya düzenleyebilir. grup oturumları maksimum beş katılımcıya kadar destekler. yazılımı kullanmak için web siteye spotify hesabınız ile giriş yapmalısınız.

---

## tasarım ve geliştirme

- [@burakbbyrmm](https://www.instagram.com/burakbbyrmm)


### kullanılan teknolojiler

- react.js
- next.js
- node.js
- express.js
- socket.io
- redux
- bootstrap
- spotify web api

## kullanıcı senaryoları

- grup oturumu oluşturan kullanıcı, arkadaşlarını oturuma davet eder ve arkadaşları oturuma katılır
- daha sonra oturumdaki herkesin düzenleyebileceği ve spotify aracılığıyla tüm cihazlarda senkronize olarak çalınan aktif bir şarkı sırası oluşur

## kurulum:

<details>
<summary>adımlar...</summary>
<br />

### ana kurulum

bu, [next.js](https://nextjs.org/) ile oluşturulmuş bir [`react`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) projesidir.

web sitesini kurmaya başlamadan önce, spotify'ın istediği gereksinimleri gerçekleştirmelisiniz:

1. [spotify geliştirici portalı](https://developer.spotify.com/my-applications/)'nda bir uygulama oluşturun

2. spotify uygulama ayarları kısmındaki geri yanıt kısmına http://localhost:3000/auth/callback (geliştiriciler için) ve <domain.com>/auth/callback (herkese açık paylaşım için) girin

3. proje klasörüne `.env` dosyası oluşturun ve aşağıdaki parametreleri tamamlayın;

   - `HOST`
   - `CLIENT_ID`
   - `CLIENT_SECRET`

örnek:

```
HOST=http://localhost:3000
CLIENT_ID=<client_id>
CLIENT_SECRET=<client_secret>
```

`CLIENT_ID` ve `CLIENT_SECRET` değerleri uygulama ayarları menüsünde mevcut

### dosya kurulumu

gereken modülleri indirmek için `npm install` komutunu çalıştırın.

### yürütme

projeyi geliştirici modunda başlatmak için, `npm run dev`.

herkese açık paylaşım için, `npm run build && npm run start`.

</details>
