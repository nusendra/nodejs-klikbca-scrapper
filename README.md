# nodejs-bca-scraper

Plugin untuk membantu anda mendapatkan informasi saldo terakhir rekening BCA anda serta mutasi rekening BCA anda pada hari itu melalui KlikBCA.

## Cara Install

```bash
npm install --save nodejs-klikbca-scrapper
```

atau

```bash
yarn add nodejs-klikbca-scrapper
```

## Penggunaan

```javascript
const bca = require('nodejs-klikbca-scrapper');
```

### Cek Saldo Terakhir

```javascript
bca
  .getBalance(USERNAME, PASSWORD)
  .then(res => {
    console.log('saldo ', res);
  })
  .catch(err => {
    console.log('error ', err);
  });
```

### Cek Settlement Pada Hari Itu

```javascript
bca
  .getSettlement(USERNAME, PASSWORD)
  .then(res => {
    console.log('settlement ', res);
  })
  .catch(err => {
    console.log('error ', err);
  });
```

# License

MIT

# Author

[Achmad Apriady](mailto:achmad.apriady@gmail.com)


# Modified by 

[Nusendra Hanggarawan](mailto:admin@nusendra.com)
