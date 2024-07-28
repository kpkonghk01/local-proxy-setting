# Demo local setting

Using [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension to proxy anything

to sign a cert:

```bash
# In your user home directory
brew install mkcert
mkcert -install
# install.pem, install-key.pem will be created, keep it safe

# In project root
mkcert -key-file ./.cert/key.pem -cert-file ./.cert/cert.pem "hkdev.com"
```

to use the demo setting:

```bash
cp .vscode/settings-demo.json .vscode/settings.json
```