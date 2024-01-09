# torrenter
Stream or download movies, animes from torrent sites from your terminal

#### I highly recommend using a curl version which supports http3 like https://github.com/stunnel/static-curl/releases if u don't wanna use a vpn
- download & extract the binary & rename it to smth like curl3 then move it to /usr/local/bin/
- In ur .zprofile, .bash_profile, or .fish_profile ?
````sh
export HTTP3_CURL_CMD='curl3 -s --http3'
````

- OR in ~/.config/torrenter/config
````sh
http3_curl_cmd='curl3 -s --http3'
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
- fzf
- rofi (alternative menu to fzf without terminal)
- dmenu (alternative menu without terminal)
- webtorrent-cli (Streaming torrent)
- peerflix (alternative to webtorrent)
- mpv (Streaming video)
- aria2 (Optimal, for downloading)
