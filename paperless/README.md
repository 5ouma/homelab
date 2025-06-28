<!-- name: 🍃 Paperless -->
<h1 align="center"><a href="https://docs.paperless-ngx.com">Paperless</a></h1>

<div align="center">

**🍃 Document management system that transforms your physical documents into a
searchable online archive**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |      Name      |           Value           |
   | :------------: | :-----------------------: |
   | `DB_PASSWORD`  | Random Database Password  |
   |  `BACKUP_DIR`  |  Local Backup Directory   |
   | `TUNNEL_TOKEN` | [Cloudflare Tunnel Token] |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```
