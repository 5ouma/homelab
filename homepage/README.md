<h1 align="center"><a href="https://gethomepage.dev">Homepage</a></h1>

<div align="center">

**🏠 Highly customizable homepage with Docker and service API integrations**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |                 Name                  |              Value              |
   | :-----------------------------------: | :-----------------------------: |
   | `HOMEPAGE_VAR_SPEEDTEST_TRACKER_HOST` | Host Name for Speedtest Tracker |
   |      `HOMEPAGE_VAR_IMMICH_HOST`       |      Host Name for Immich       |
   |     `HOMEPAGE_VAR_IMMICH_API_KEY`     |        [Immich API Key]         |
   |            `TUNNEL_TOKEN`             |    [Cloudflare Tunnel Token]    |

   [Immich API Key]: https://immich.app/docs/features/command-line-interface#obtain-the-api-key
   [Cloudflare Tunnel Token]: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

2. 🚀 Start the Docker Compose

   ```shell
   docker compose up -d
   ```
