# Torrent / YouTube Leecher 🔥🤖

A Telegram Torrent, youtube-dl Leecher, and rClone / Telegram Uploader!
A Torrent, youtube-dl Leecher, and Uploader!

## installing

### The Easy Way

[![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run)


[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

### The Legacy Way
Simply clone the repository and run the main file:

```sh
git clone https://github.com/SpEcHiDe/PublicLeech.git
cd PublicLeech
python3 -m venv venv
. ./venv/bin/activate
pip install -r requirements.txt
# <Create config.py appropriately>
python3 -m tobrot
```

### an example config.py 👇
```py
from tobrot.sample_config import Config

class Config(Config):
  TG_BOT_TOKEN = "123456:ABC-DEF1234ghIkl-zyx57W2v1u123ew11"
  # These example values won't work. You must get your own app_id and
  # api_hash from https://my.telegram.org, under API Development.
  APP_ID = 6
  API_HASH = "eb06d4abfb49dc3eeb1aeb98ae0f581e"
  # please read https://t.me/c/1279877202/74
  # if you have not read the above README
  AUTH_CHANNEL = [-1001234567890]
    TG_BOT_TOKEN = "123456:ABC-DEF1234ghIkl-zyx57W2v1u123ew11"
    # These example values won't work. You must get your own app_id and
    # api_hash from https://my.telegram.org, under API Development.
    APP_ID = 6
    API_HASH = "eb06d4abfb49dc3eeb1aeb98ae0f581e"
    # please read https://t.me/c/1279877202/74
    # if you have not read the above README
    AUTH_CHANNEL = [
        -1001234567890,
        7351948,
        -456790
    ]
```

### Variable Explanations

##### Mandatory Variables

* `TG_BOT_TOKEN`: Create a bot using [@BotFather](https://telegram.dog/BotFather), and get the Telegram API token.

* `APP_ID`
* `API_HASH`: Get these two values from [my.telegram.org/apps](https://my.telegram.org/apps).
  * N.B.: if Telegram is blocked by your ISP, try our [Telegram bot](https://telegram.dog/UseTGXBot) to get the IDs.

* `AUTH_CHANNEL`:
Create a Super Group in Telegram, add `@GoogleIMGBot` to the group, and send /id in the chat, to get this value.
You can add multiple IDs seperated by space.

##### Optional Configuration Variables

* `DOWNLOAD_LOCATION`

* `SHOULD_USE_BUTTONS`: because, [BlameTelegram](https://t.me/c/1494623325/5603)

* `ARIA_TWO_STARTED_PORT`: The port on which aria2c daemon must START. This should be an integer, between 1001 and 65535.

* `EDIT_SLEEP_TIME_OUT`: The number of seconds to sleep after editing a Telegram message.

* `MAX_TIME_TO_WAIT_FOR_TORRENTS_TO_START`: The number of seconds to wait before auto-cancelling a dead link.

* `FINISHED_PROGRESS_STR`: any character(s) that might be displayed in the progress string.

* `UN_FINISHED_PROGRESS_STR`: any character(s) that might be displayed in the progress string.

* `TG_OFFENSIVE_API`: ~~DO NOT USE THIS~~.

* `R_CLONE_CONF_URI`:
![a help, maybe](https://telegra.ph/file/073bcbc0b69b03d75ea04.jpg)

* `DOWNLOAD_LOCATION`: optional download directory, where the temporary downloads should ideally reside.

* `MAX_FILE_SIZE`

* `TG_MAX_FILE_SIZE`

* `FREE_USER_MAX_FILE_SIZE`

* `MAX_TG_SPLIT_FILE_SIZE`

* `CHUNK_SIZE`

* `MAX_MESSAGE_LENGTH`

* `PROCESS_MAX_TIMEOUT`

* `ARIA_TWO_STARTED_PORT`

* `EDIT_SLEEP_TIME_OUT`

* `MAX_TIME_TO_WAIT_FOR_TORRENTS_TO_START`

* `FINISHED_PROGRESS_STR`

* `UN_FINISHED_PROGRESS_STR`

* `TG_OFFENSIVE_API`

* `R_CLONE_CONF_URI`
![a help, maybe](https://telegra.ph/file/073bcbc0b69b03d75ea04.jpg)

* `SHOULD_USE_BUTTONS`: because, [BlameTelegram](https://t.me/c/1494623325/5603)

## Available Commands

* The available commands depends on the ENVironment / CONfig variables that is set by you.
* You can read the [Commandi](./tobrot/dinmamoc.py) file, to know about the ENVironment variables to use.


## How to Use?

* send any link, and click on the available buttons.

* if file is larger than 1500MB, [read this](https://t.me/c/1434259219/113).

* if file is a TAR archive, [read this](https://t.me/c/1434259219/104) to know how to uncompress.


## How to get `R_CLONE_CONF_URI` ?

- Start the RoBot by leaving the var empty.
- Create a rclone.conf by going to the [official website](https://rclone.org/)
- Upload the rclone.conf, in your private chat / channel**.
- Reply the `GET_RCLONE_CONF_URI` Commandi, to the uploaded file.
- RoBot will reply a monospaced text.
- Add it to the `R_CLONE_CONF_URI` ENVironment VARiable.


## Issues or Feature Requests

* search for known issues, [here](https://t.me/c/1434259219/118) or in the [GitHub Issues](https://github.com/SpEcHiDe/PublicLeech/issues).

* add issues / feature requests, [here](https://github.com/SpEcHiDe/PublicLeech/issues/new).


## Credits, and Thanks to

* [me](https://GitHub.com/SpEcHIDe/PublicLeech)
* [Dan Tès](https://telegram.dog/haskell) for his [Pyrogram Library](https://github.com/pyrogram/pyrogram)
* [Robots](https://telegram.dog/Robots) for their [@UploadBot](https://telegram.dog/UploadBot)
* [@AjeeshNair](https://telegram.dog/AjeeshNait) for his [torrent.ajee.sh](https://torrent.ajee.sh)
* [@gotstc](https://telegram.dog/gotstc), @aryanvikash, [@HasibulKabir](https://telegram.dog/HasibulKabir) for their TORRENT groups
* [rClone Team](https://github.com/rclone/rclone)
* [gautamajay52](https://github.com/gautamajay52/TorrentLeech-Gdrive)
* [![CopyLeft](https://telegra.ph/file/b514ed14d994557a724cb.jpg)](https://telegra.ph/file/fab1017e21c42a5c1e613.mp4 "CopyLeft Credit Video")
