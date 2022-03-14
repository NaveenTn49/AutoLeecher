# Telegram Torrent Leecher 

```
TESTED REPO WORKING FINE FOR ME ABUSE=BAN ON Her*ku...
```

A Telegram Torrent (and youtube-dl) Leecher based on [Pyrogram](https://github.com/pyrogram/pyrogram)

## installing

### The Easy Way

Do Not Abuse , Better Use Public Leech Groups

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)


### The Eas(iest) Way

- Install Docker by following the [official docker docs](https://docs.docker.com/engine/install/debian/)

- Start docker daemon [skip if already running]:
```sh
dockerd
```
- Build Docker image:
```sh
docker build . -t public-leech
```
- Run the image:
```sh
docker run public-leech
```

IF You want to Use this Bot Use in Closed Supergroup Avoid Giving Access to Untrusted Personal.


### The Legacy Way
Simply clone the repository and run the main file:

```sh
git clone https://github.com/NaveenTn49/AutoLeecher.git
cd AutoLeecher
virtualenv -p /usr/bin/python3 venv
. ./venv/bin/activate
pip install -r requirements.txt
# <Create conf.py appropriately>
python3 -m apdbot
```

### an example for creating conf.py 👇
```py
from apdbot.sample_con import Config

class Config(Config):
  BOT_TOKEN = ""
  APP_ID = 6
  API_HASH = "eb06d4abfb49dc3eeb1aeb98ae0f581e"
  AUTH = [-1001234567890, -1001234567891]
```

### Variable Explanations

##### Mandatory Variables

* `BOT_TOKEN`: Create a bot using [@BotFather](https://telegram.dog/BotFather), and get the Telegram API token.

* `APP_ID`
* `API_HASH`: Get these two values from [my.telegram.org/apps](https://my.telegram.org/apps).
  * N.B.: if Telegram is blocked by your ISP, try our [Telegram bot](https://telegram.dog/UseTGXBot) to get the IDs.

* `AUTH`: Create a Super Group in Telegram, add `@GoogleIMGBot` to the group, and send /id in the chat, to get this value.

##### Optional Configuration Variables

* `DOWNLOAD_LOC`

* `MAX_SIZE`

* `TG_MAX_SIZE`

* `FREE_UZR_MAX_SIZE`

* `MAX_SIZE_TO_SPLIT`

* `CHUNK_SIZE`

* `MAX_MESSAGE_LENGTH`

* `PROCESS_TIMEOUT`

* `ARIA_STARTED_PORT`

* `EDIT_SLEEP_TIME`

* `MAX_TIME_TO_WAIT_FOR_START`

* `FINISHED_PROGRESS_STR`

* `UN_FINISHED_PROGRESS_STR`

* `CUSTOM_NAME`

## Variables to Edit Commands

* `LEECH_CMD`

* `YTDL_CMD`

* `CANCEL_CMD`

* `STATUS_CMD`

* `LOG_CMD`

* `SAVE_CMD`

* `CLEAR_CMD`

* `UPLOAD_CMD`

* `EXEC_CMD `

* `HELP_CMD`

## Available Commands

* `/ytdl`: This command should be used as reply to a [supported link](https://ytdl-org.github.io/youtube-dl/supportedsites.html)

* `/pytdl`: This command should be used as reply to a youtube playlist

* `/leech`: This command should be used as reply to a magnetic link, a torrent link, or a direct link. [this command will SPAM the chat and send the downloads a seperate files, if there is more than one file, in the specified torrent]

* `/leech archive`: This command should be used as reply to a magnetic link, a torrent link, or a direct link. [This command will create a .tar.gz file of the output directory, and send the files in the chat, splited into PARTS of 1024MiB each, due to Telegram limitations]

* `/leech unzip`: This command should be used as reply to a magnetic link, a torrent link, or a direct link. [This command will Unzip the RAR, TAR, ZIP Files]

## How to Use?

* send any one of the available command, as a reply to a valid link.

* if file is larger than 2000MB, [read this](https://t.me/naveenleech49_bot).

* if file is a TAR archive, [read this](https://t.me/naveenleech49_bot) to know how to uncompress.


## Issues or Feature Requests

* search for known issues, [here](https://t.me/naveenleech49_bot).

* add issues / feature requests, [here](https://github.com/SpEcHiDe/PublicLeech/issues/new).
