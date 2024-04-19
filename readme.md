# Laboratorium 6

### Budowanie obrazu:

`docker build --ssh default  -f Dockerfile_z1 -t ghcr.io/measter9/lab6:v0 .`

argument `--ssh default` pobiera dane logowania ssh zapisane na lokalnej maszynie

### Uruchamianie:

`docker run -h=myhostanme -d --name lab6 -p 3000:3000 ghcr.io/measter9/lab6:v0`

efekt dzialania analogiczny jak w lab.5

### Przesłanie na repozytorium ghcr.io

`docker push ghcr.io/measter9/lab6:v0`
