# Self-hosted blog

- Halo: https://github.com/halo-dev/halo
- Cloudfare tunnel: https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

## How to
- Register Cloudfare account: https://www.cloudflare.com/en-ca/
- Turn on Zero trust
- Make sure you have a domain name ready and set it up under `Networks -> Tunnel -> Public hostname`. URL should be service:port. eg. `halo:8090`
- Create .env and replace value with your own token `CLOUDFARE_TUNNEL_TOKEN=yourtokengoeshere`
- Run `docker compose up -d` to start the container 
- Visit your domain name and you should see the blog
