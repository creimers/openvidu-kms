# openvidu server evaluation

## quickstart

- edit `openvidu.publicurl` in `docker-compose.yml`. The hostname should be your local IP address.
- `docker-compose up`
- create a session called `sm400` via the API
- add an rstp stream to the session via the API
- make sure your browser accepts the TLS certificate by navigating to `local_ip:4443`
- run `yarn start` and open your browser at `local_ip:3000`
