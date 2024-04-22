<h1 align="center"><a href="https://immich.app">Immich</a></h1>

<div align="center">

**🌸 Self-hosted photo and video management solution**

![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/5ouma/immich?style=flat-square)
![GitHub repo size](https://img.shields.io/github/repo-size/5ouma/immich?style=flat-square)
[![GitHub last commit](https://img.shields.io/github/last-commit/5ouma/immich?style=flat-square)](https://github.com/5ouma/immich/commit/HEAD)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/5ouma/immich?style=flat-square)](https://github.com/5ouma/immich/commits/main)

</div>

<br /><br />

## 🔐 Requirements

- ### 🐳 Docker Compose

  > I use [🔮 OrbStack](https://orbstack.dev).

<br /><br />

## 🔧 Setup

1. ### 📋 Clone this Repository

   ```shell
   git clone https://github.com/5ouma/immich.git
   ```

   <br />

2. ### 🏔️ Set the Environment Variables in [`.env`](../.env)

   | Variable Name |          Value           |
   | :-----------: | :----------------------: |
   |  DB_PASSWORD  | Random Database Password |
   |  TS_AUTHKEY   |   [Tailscale Auth Key]   |

   [Tailscale Auth Key]: https://login.tailscale.com/admin/settings/keys

   <br />

3. ### 🚀 Start the Docker Compose

   ```shell
   docker compose up -d
   ```
