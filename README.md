# openvidu server evaluation

## quickstart

- edit `openvidu.publicurl` in `docker-compose.yml`. The hostname should be your local IP address.
- run `docker-compose up`
- create a session called `sm400` via the API
- add an rtsp stream to the session via the API like so:

```json
{
  "type": "IPCAM",
  "rtspUri": "rtsp://192.168.1.106:8554/unicast",
  "adaptativeBitrate": true,
  "onlyPlayWithSubscribers": true
}
```

- make sure your browser accepts the TLS certificate by navigating to `https://local_ip:4443`
- run `cd client`, `yarn install` and `yarn start`, then open your browser at `http://local_ip:3000`
