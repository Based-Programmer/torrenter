## torrenter
Stream torrent movies animes &amp; download them for your terminal

# Install

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
pnpm -g install webtorrent-cli && \
curl -L 'https://github.com/Based-Programmer/torrenter/raw/main/torrenter' -O && \
chmod +x torrenter && \
mv torrenter $PREFIX/bin/
```
## Dependencies

- curl
- fzf
- rofi (alternative menu to fzf without terminal)
- dmenu (alternative menu without terminal)
- webtorrent-cli (Streaming torrent)
- peerflix (alternative to webtorrent)
- mpv (Streaming video)
- aria2 (Optimal, for downloading)
