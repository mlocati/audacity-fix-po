FROM debian:bookworm

RUN apt-get update -q \
    && apt-get upgrade -qy \
    && apt-get install -qy git gettext \
    && rm -rf /var/lib/apt/lists/*

COPY --chmod=0755 entrypoint /

ENTRYPOINT [ "/entrypoint" ]
