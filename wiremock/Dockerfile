FROM rodolpheche/wiremock

COPY stubs /home/wiremock

RUN addgroup --gid 2000 --system appgroup && \
    adduser --uid 2000 --system appuser --gid 2000


USER 200
