# Laboratorium 6

### Budowanie obrazu:


`buildctl build --ssh default --frontend=dockerfile.v0 --local context=pawcho6 --local dockerfile=pawcho6 --opt filename=./Dockerfile_z1 --output type=image,name=ghcr.io/measter9/lab6:v1,push=true`

argument `--ssh default` pobiera dane logowania ssh zapisane na lokalnej maszynie

### Uruchamianie:

`docker run -h=myhostanme -d --name lab6 -p 3000:3000 ghcr.io/measter9/lab6:v1`

efekt dzialania analogiczny jak w lab.5
