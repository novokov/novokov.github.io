---
layout: post
title: "SSL ошибка при парсинге"
categories: python
---

Ошибка SSL при парсинге 

```
-> <urlopen error [SSL: CERTIFICATE_VERIFY_FAILED]
-> certificate verify failed: unable to get local issuer
-> certificate (_ssl.c:1076)>
```

Ошибка говорит об отсутствии сертификата 

Чинится так. Запускаем команду в bash и готово

```bash
open /Applications/Python\ 3.7/Install\ Certificates.command
```