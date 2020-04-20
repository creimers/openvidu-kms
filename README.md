# openvidu server evaluation

## quickstart

- edit `openvidu.publicurl` in `docker-compose.yml`. The hostname should be your LAN IP address.
- run `docker-compose up`
- create a session called `sm400` via the API. Refer to [postman_collection.json](./postman_collection.json).
- add an rtsp stream to the session via the API. Refer to [postman_collection.json](./postman_collection.json).
- make sure your browser accepts the TLS certificate by navigating to `https://LAN_ip:4443`.
- run `cd client`, `yarn install` and `yarn start`, then open your browser at `http://LAN_ip:3000`.
