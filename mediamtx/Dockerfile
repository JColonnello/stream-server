FROM aler9/rtsp-simple-server AS rtsp
FROM alpine:3.12
RUN apk add --no-cache ffmpeg
COPY --from=rtsp /mediamtx /
COPY --from=rtsp /mediamtx.yml /
ENTRYPOINT [ "/mediamtx" ]