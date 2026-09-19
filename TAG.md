
# Docker 
use version specific; Here `arm-64 aarch64` no `amd64. No builderX used. 

- Image build: rubyfever
## Tag
docker tag rubyrailsfever cureerel/rubyrailsfever:latest
docker tag rubyrailsfever cureerel/rubyrailsfever:1.0.0  

## Push
docker push cureerel/rubyrailsfever:latest
docker push cureerel/rubyrailsfever:1.0.0


## build

#### --target runtime   for multi
```bash
docker build \
  -f Dockerfile.dev \
  -t rubyrailsfever:1.0.0 \
  .
```

```bash
docker run -d \
  -p 3000:3000 \
  --name rubyrailsfever \
  rubyrailsfever:1.0.0
```


## check
```bash
docker images rubyrailsfever
```