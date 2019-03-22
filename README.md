[pb](https://github.com/ptpb/pb) is a self-hosted pastebin and url shortening service.

This docker config uses [this image](https://hub.docker.com/r/ptpb/pb/).

# Setup

This relies on my [base docker services](https://github.com/StarlitGhost/selfhost-base).  
You'll want to symlink that project's .env file into this project's directory and set `DOMAIN_SHORTENER` in it (or edit docker-compose.yml to use a subdomain of `${DOMAIN_BASE}` - whatever makes sense for you).

Once that's done you can just spin it up with `docker-compose up -d`. Boom, service working.

Out of the box, pb only accepts pastes and URLs via API.  
Optionally you can set up a friendly web form for this, the process for that is described in the README for [pbwww](https://github.com/DesertBot/pbwww).
