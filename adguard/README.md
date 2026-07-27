<!-- name: 🛡️ AdGuard Home -->
<h1 align="center"><a href="https://adguard.com/adguard-home.html">AdGuard Home</a></h1>

<div align="center">

**🛡️ Network-based solution for blocking ads and trackers**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |      Name      |           Value           |
   | :------------: | :-----------------------: |
   |  `PASSPHRASE`  |   Random GPG Passphrase   |
   |  `BACKUP_DIR`  |  Local Backup Directory   |
   | `TUNNEL_TOKEN` | [Cloudflare Tunnel Token] |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 📝 Enable insecure DoH

   ```sh
   yq -i '.http.doh.insecure_enabled = true' AdGuardHome.yaml
   ```

3. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```
