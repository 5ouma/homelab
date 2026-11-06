<!-- name: 🍃 Paperless -->
<h1 align="center"><a href="https://docs.paperless-ngx.com">Paperless</a></h1>

<div align="center">

**🍃 Document management system that transforms your physical documents into a
searchable online archive**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |         Name         |            Value             |
   | :------------------: | :--------------------------: |
   |  `OIDC_ISSUER_URL`   |  OpenID Connect Issuer URL   |
   |   `OIDC_CLIENT_ID`   |   OpenID Connect Client ID   |
   | `OIDC_CLIENT_SECRET` | OpenID Connect Client Secret |
   |   `PAPERLESS_URL`    |        Paperless URL         |
   |    `DB_PASSWORD`     |   Random Database Password   |
   |     `BACKUP_DIR`     |    Local Backup Directory    |
   |    `TUNNEL_TOKEN`    |  [Cloudflare Tunnel Token]   |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```

<br />

## ⚙️ Regenerate Assets

```sh
docker compose exec webserver bash -c 'document_thumbnails'
docker compose exec webserver bash -c 'document_archiver --overwrite'
```
