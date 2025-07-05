<!-- name: 🌸 Immich -->
<h1 align="center"><a href="https://immich.app">Immich</a></h1>

<div align="center">

**🌸 Self-hosted photo and video management solution**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |       Name        |             Value              |
   | :---------------: | :----------------------------: |
   |   `DB_PASSWORD`   |    Random Database Password    |
   |   `WEBDAV_URL`    |    URL of the WebDAV server    |
   |   `WEBDAV_PATH`   |   Path to the WebDAV server    |
   | `WEBDAV_USERNAME` | Username for the WebDAV server |
   | `WEBDAV_PASSWORD` | Password for the WebDAV server |
   |   `BACKUP_DIR`    |     Local Backup Directory     |
   |  `TUNNEL_TOKEN`   |   [Cloudflare Tunnel Token]    |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```
