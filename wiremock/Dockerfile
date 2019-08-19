FROM rodolpheche/wiremock

RUN addgroup --gid 2000 --system appgroup && \
    adduser --uid 2000 --system appuser --gid 2000


WORKDIR /wiremock

COPY stubs /home/wiremock

RUN chown -R appuser:appgroup /wiremock

USER 2000

