# Streaming server
---
## Run
```sh
docker compose up
```

## Testing

Publish a looping video
```sh
ffmpeg -re -stream_loop -1 -i "<Video file>" -c copy -f rtsp rtsp://localhost:8554/mystream
```