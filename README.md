# michalliska.com

Osobná stránka Michala Líšku. Statický web, jeden HTML súbor.

- `index.html` — celá stránka (CSS aj JS inline)
- `assets/portrait.jpg` — hero fotka (orezaná), `portrait_full.jpg` je originál a nedeployuje sa
- `.htaccess` — HTTPS redirect + short linky (`/in`, `/ig`, `/yt`, `/setup` a aliasy)

## Hosting

- Doména: Hostinger (michalliska.com)
- Hosting: Websupport, docroot `/michalliska.com/web`
- Deploy: automaticky pri push na `main` cez GitHub Actions (FTP, secrets `FTP_SERVER`, `FTP_USERNAME`, `FTP_PASSWORD`, `FTP_SERVER_DIR`)

## Lokálny náhľad

```
python3 -m http.server 8741
```

Debug parametre: `?static=1` vypne animácie, `&section=stats|pillars|work|contact` izoluje sekciu.
