<h1 align="center"><a href="https://speedtest-tracker.dev">Speedtest Tracker</a></h1>

<div align="center">

**🐇 Self-hosted internet performance tracking application**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |      Name      |           Value           |
   | :------------: | :-----------------------: |
   |   `APP_KEY`    |     [Encryption Key]      |
   | `DB_PASSWORD`  | Random Database Password  |
   | `TUNNEL_TOKEN` | [Cloudflare Tunnel Token] |

   [Encryption Key]: https://speedtest-tracker.dev
   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```shell
   docker compose up -d
   ```
