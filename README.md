# torrenter
Stream or download movies, animes from torrent sites from your terminal

#### Update
- `eztv` doesn't work either, good alternative is `yts`

#### Pro Tip
- while playing, reload the video if it gets stuck
- to do that bind a key in mpv `input.conf`
````
p      write-watch-later-config; loadfile "${path}"
````

## Install

#### Linux
- First of all update & install the following [dependencies](#Dependencies) listed below

````sh
curl -L 'https://github.com/Based-Programmer/torrenter/raw/main/torrenter' -O && \
chmod +x torrenter && \
sudo mv torrenter /usr/local/bin/
````

#### Termux

```sh
pkg up -y && \
pkg in curl fzf aria2 nodejs && \
npm -g install webtorrent-cli && \
curl -L 'https://github.com/Based-Programmer/torrenter/raw/main/torrenter' -O && \
chmod +x torrenter && \
mv torrenter $PREFIX/bin/
```

## Dependencies

- curl
- fzf (menu)
- webtorrent-cli (Streaming torrent)
- mpv (best media player ever)

## Optimal Dependencies

- rofi (alternative menu to fzf without terminal)
- dmenu (alternative menu without terminal)
- peerflix (alternative to webtorrent)
- aria2 (for downloading)
- libnotify (only for alternative menus)
