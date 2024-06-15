<h1 align="center"><a href="https://speedtest-tracker.dev/">Speedtest Tracker</a></h1>

<div align="center">

**🐇 Self-hosted internet performance tracking application**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |     Name      |          Value           |
   | :-----------: | :----------------------: |
   |   `APP_KEY`   |     [Encryption key]     |
   | `DB_PASSWORD` | Random Database Password |
   | `TS_AUTHKEY`  |   [Tailscale Auth Key]   |

   [Encryption key]: https://speedtest-tracker.dev
   [Tailscale Auth Key]: https://login.tailscale.com/admin/settings/keys

2. 🚀 Start the Docker Compose

   ```shell
   docker compose up -d
   ```
