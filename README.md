# Caddy test
## Run test nginx
`
docker run -d -p 1023:80 nginx
`
## Proxy nginx
`
docker run -d  -v $(pwd)/Caddyfile:/etc/Caddyfile -v $HOME/.caddy:/root/.caddy  -p 80:80 -p 443:443  abiosoft/caddy
`
