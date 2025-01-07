<h1 align="center"><a href="https://immich.app">Immich</a></h1>

<div align="center">

**🌸 Self-hosted photo and video management solution**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |       Name       |           Value           |
   | :--------------: | :-----------------------: |
   |  `DB_PASSWORD`   | Random Database Password  |
   | `R2_BUCKET_NAME` | Cloudflare R2 Bucket Name |
   |   `BACKUP_DIR`   |  Local Backup Directory   |
   |  `TUNNEL_TOKEN`  | [Cloudflare Tunnel Token] |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```

<!-- name: 🌸 Immich -->
