# Dino Flathub

How to update

```sh
# Download latest release from https://github.com/dino/dino/releases
wget https://github.com/dino/dino/releases/download/v0.5.0/dino-0.5.0.tar.gz
wget https://github.com/dino/dino/releases/download/v0.5.0/dino-0.5.0.tar.gz.asc

# Verify the signed archive
gpg --locate-key release-signing@dino.im
gpg --verify dino-0.5.0.tar.gz.asc

# Download the manifest from upstream
curl -O https://raw.githubusercontent.com/dino/dino/master/im.dino.Dino.json

sha256sum dino-0.5.0.tar.gz
# Update the type, url and sha256 of the dino module in im.dino.Dino.json
```
