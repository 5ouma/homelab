<!-- name: 🍦 Soft Serve -->
<h1 align="center">
<a href="https://github.com/charmbracelet/soft-serve">Soft Serve</a>
</h1>

<div align="center">

**🍦 The mighty, self-hostable Git server for the command line**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |              Name               |              Value               |
   | :-----------------------------: | :------------------------------: |
   | `SOFT_SERVE_INITIAL_ADMIN_KEYS` |          SSH Public Key          |
   |        `SOFT_SERVE_NAME`        | Name will be Displayed in the UI |
   |       `SOFT_SERVE_DOMAIN`       |     Domain to Serve Publicly     |
   |         `TUNNEL_TOKEN`          |    [Cloudflare Tunnel Token]     |

   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```

3. 🐙 Import GitHub repositories and Gists as mirrors

   > [!IMPORTANT]
   > You need GitHub CLI and jq installed.

   ```sh
   ./scripts/mirror git.example.com
   ```

   > [!NOTE]
   > Soft Serve's SSH public key must be added to your GitHub account
   > to pull private repositories.
   >
   > ```sh
   > docker compose exec server bash -c 'cat /soft-serve/ssh/soft_serve_client_ed25519.pub'
   > ```
