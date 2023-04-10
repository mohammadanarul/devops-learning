### caddy and mkcert configaration for `macbook`

**step-1**
```
brew install mkcert
brew install nss
mkcert -install
```

**step-2**
```
mkcert -cert-file local.crt -key-file local.key "local.localhost" "dev.localhost"
```

### caddy and mkcert configaration for `linux`

**step-1**
```
sudo apt install libnss3-tools

curl -JLO "https://dl.filippo.io/mkcert/latest?for=linux/amd64"

chmod +x mkcert-v*-linux-amd64

sudo cp mkcert-v*-linux-amd64 /usr/local/bin/mkcert

mkcert -install
```
**step-2**
```
mkcert -cert-file local.crt -key-file local.key "local.localhost" "dev.localhost"
```