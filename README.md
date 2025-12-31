# a easy & minimal proxy tool for linux command line

a very minimal command line tool to manage your proxy. NO GUI, NO complex config, NO system proxy, NO shit. Just designed for linux terminal user!

It does one simple job: local socks5 => shadowrocket subscription. That's it.

## Demo Video: Recommended Usage

> Enjoy with SwitchyOmega / ProxyChains / Graftcp ...

![Demo Video](.res/recording-proxy-fish-usage.avif)

## Installation

> Dependency: `sudo pacman -S fish python v2ray shadowsocks-rust jq`

1. Copy `proxy.fish` and `lib` into your PATH.
2. (Optional) Copy `completions` into `~/.config/fish/completions`.
3. Enjoy

## supported scenario

1. shadowrocket format subscription url (base64 encoded lines)
2. protocol: v2ray (vmess, vless), shadowsocks, ssh proxy
3. will use native shadowsocks client is possible, v2ray as fallback. (shadowsocks-rust, shadowsocks-libev, shadowsocks-python supported)
4. common vless args supported (such as allow-insecure, SNI spoof), reality or other x-ray trick not supported

