<!-- name: 🔒 Pocket ID -->
<h1 align="center"><a href="https://pocket-id.org">Pocket ID</a></h1>

<div align="center">

**🔒 The most user-friendly OpenID Connect Certified™ and OAuth 2.0 provider**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |      Name      |           Value           |
   | :------------: | :-----------------------: |
   |   `APP_URL`    |    Your Pocket ID URL     |
   | `DB_PASSWORD`  | Random Database Password  |
   |  `BACKUP_DIR`  |  Local Backup Directory   |
   | `TUNNEL_TOKEN` | [Cloudflare Tunnel Token] |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```
