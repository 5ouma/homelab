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

3. 🐙 Import GitHub repositories as mirrors

   ```sh
   domain=''
   while read -r repo; do
     name=$(echo "$repo" | cut -d, -f1)
     url=$(echo "$repo" | cut -d, -f2)
     description=$(echo "$repo" | cut -d, -f3)
     ssh -n "$domain" repo import -m "$name" -d "$description" "$url"
   done < <(gh repo list --source --json 'name,description,url' --jq '.[] | [.name,.url,.description] | @csv')
   ```
