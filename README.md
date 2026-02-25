### homelab

> [!NOTE]
> Right now, I'm in the middle of restructuring my setup
> so the repo is a bit of a mess.

These are just a few docker compose containers running at a homelab,
nothing much to see here.

To run these, get docker-compose.

Stuff in `quadlets/` are quadlet versions of the docker compose files being
rewritten to play well with podman/systemd ecosystem. Right now, only immich
and jellyfin are there.

Place the files in `quadlets/` at `~/.config/containers/systemd` and run
`systemctl --user daemon-reload` to reload the config.

> [!IMPORTANT]
> Rename .env.example to .env and configure the values as required before
> starting up the containers
