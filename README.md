# setup v2ray

Setup V2Ray for GitHub actions.

```yaml
- uses: wangsijie/setup-v2ray@v1
    with:
      config-base64: ${{ secrets.CONFIG }}
```

works like:

```yaml
- run: curl ip.sb # see if it is the proxy server's ip
  env:
    http_proxy: "127.0.0.1:1080"
```

## config

`config-base64` is base64 encoded string of V2Ray's `config.json`
