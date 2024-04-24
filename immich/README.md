<h1 align="center"><a href="https://immich.app">Immich</a></h1>

<div align="center">

**🌸 Self-hosted photo and video management solution**

</div>

<br /><br />

## 🔧 Setup

1. ### 🏔️ Set the Environment Variables in [`.env`](./.env)

   | Variable Name |          Value           |
   | :-----------: | :----------------------: |
   |  DB_PASSWORD  | Random Database Password |
   |  TS_AUTHKEY   |   [Tailscale Auth Key]   |

   [Tailscale Auth Key]: https://login.tailscale.com/admin/settings/keys

   <br />

2. ### 🚀 Start the Docker Compose

   ```shell
   docker compose up -d
   ```
