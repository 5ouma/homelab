<h1 align="center"><a href="https://misskey-hub.net">Misskey</a></h1>

<div align="center">

**🌐 Interplanetary micro-blogging platform**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |      Name      |           Value           |
   | :------------: | :-----------------------: |
   | `MISSKEY_URL`  |        Misskey URL        |
   | `DB_PASSWORD`  | Random Database Password  |
   | `TUNNEL_TOKEN` | [Cloudflare Tunnel Token] |

[Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

1. 🚀 Start the Docker Compose

   ```shell
   docker compose up -d
   ```
