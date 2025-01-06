<h1 align="center">
<a href="https://github.com/mbentley/docker-timemachine">Time Machine</a>
</h1>

<div align="center">

**⏱️ Docker image to run Samba to provide a compatible Time Machine for macOS**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |          Name          |                   Value                   |
   | :--------------------: | :---------------------------------------: |
   |     `TM_USERNAME`      |             Username Runs as              |
   |     `TM_PASSWORD`      |           Password for the User           |
   |    `TM_SHARE_NAME`     |            Shared Volume Name             |
   | `TM_VOLUME_SIZE_LIMIT` | Maximum Size of the Backup ([Samba Docs]) |

   [Samba Docs]: https://www.samba.org/samba/docs/current/man-html/vfs_fruit.8

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```
