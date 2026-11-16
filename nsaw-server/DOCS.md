# not-so-advanced-war server

Runs `nsaw-server`, the authoritative WebSocket server for online matches.

Join from the game with the launch argument
`--server=ws://<home-assistant-ip>:7878` (change the host port under
*Network* if 7878 is taken).

## Options

- **seed** (optional): map seed. Leave empty for a random map on every start.
- **record_matches**: record every match as JSON Lines to
  `/addon_configs/<id>_nsaw_server/matches` (reachable through the Samba
  add-on's `addon_configs` share). Included in Home Assistant backups.
