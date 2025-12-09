Description:
    This contains config for running headscale server with Headplane UI for managing and Caddy to reverse proxy
    
Start the system with:
    docker compose up -d

Next steps:
- Headplane UI accessible at: https://vpn.abherifintech.publicvm.com/admin
- To login with new API Key, run the command in the headscale server in the project root folder: docker exec -it headscale headscale apikeys create

Adding a new server to VPN:
- Open headplane
- Go to Settings > Manage auth keys. Here you can create or re-use existing key

Common commands
- List all nodes: docker exec -it headscale headscale nodes list