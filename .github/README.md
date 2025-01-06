<h1 align="center">HomeLab</h1>

<div align="center">

**🥼 Self-hosted personal laboratory**

![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/5ouma/homelab?style=flat-square)
![GitHub repo size](https://img.shields.io/github/repo-size/5ouma/homelab?style=flat-square)
[![GitHub last commit](https://img.shields.io/github/last-commit/5ouma/homelab?style=flat-square)](https://github.com/5ouma/homelab/commit/HEAD)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/5ouma/homelab?style=flat-square)](https://github.com/5ouma/homelab/commits/main)
<br />
[![Test](https://img.shields.io/github/actions/workflow/status/5ouma/homelab/test.yml?label=test&style=flat-square)](https://github.com/5ouma/homelab/actions/workflows/test.yml)
[![Deploy](https://img.shields.io/github/actions/workflow/status/5ouma/homelab/deploy.yml?label=deploy&style=flat-square)](https://github.com/5ouma/homelab/actions/workflows/deploy.yml)

</div>

<br /><br />

## 🔐 Requirements

- 🐳 Docker Compose

  > I use [🔮 OrbStack](https://orbstack.dev).

<br /><br />

## 🔧 Setup

1. 📋 Clone this Repository

   ```sh
   git clone https://github.com/5ouma/homelab.git
   ```

2. 🏔️ Copy the [`.env.tmpl`](../.env.tmpl) file to `.env` and Edit it

   |          Name           |              Value              |
   | :---------------------: | :-----------------------------: |
   |   `AWS_ACCESS_KEY_ID`   |   Cloudflare R2 Access Key ID   |
   | `AWS_SECRET_ACCESS_KEY` | Cloudflare R2 Secret Access Key |
   |     `AWS_ENDPOINT`      |  Cloudflare R2 Endpoint Domain  |

3. 📝 Follow the instructions below

   - [🌸 **Immich**](../immich)
   - [🪐 **Misskey**](../misskey)
   - [🐇 **Speedtest Tracker**](../speedtest-tracker)
   - [⏱️ **Time Machine**](../timemachine)

<br />

## 💾 Restoring Data

1. 🗝️ Decrypt the Data

   ```sh
   # Your database password
   gpg -o ./backup.tar.gz -d /path/to/backup.tar.gz.gpg
   tar -xzf ./backup.tar.gz
   ```

2. 🐘 Copy the Database

   ```sh
   docker compose create
   docker compose start database
   docker compose cp ./backup/service.sql database:/tmp/backup.sql
   docker compose exec database bash -c 'psql -d "$POSTGRES_DB" -U "$POSTGRES_USER" -f /tmp/backup.sql'
   ```
