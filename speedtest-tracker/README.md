<!-- name: 🐇 Speedtest Tracker -->
<h1 align="center"><a href="https://speedtest-tracker.dev">Speedtest Tracker</a></h1>

<div align="center">

**🐇 Self-hosted internet performance tracking application**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |      Name      |                     Value                      |
   | :------------: | :--------------------------------------------: |
   |   `APP_KEY`    | `echo -n 'base64:' && openssl rand -base64 32` |
   | `DB_PASSWORD`  |            Random Database Password            |
   |  `BACKUP_DIR`  |             Local Backup Directory             |
   | `TUNNEL_TOKEN` |           [Cloudflare Tunnel Token]            |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```
