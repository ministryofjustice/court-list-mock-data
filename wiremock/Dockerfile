FROM rodolpheche/wiremock

RUN addgroup --gid 2000 --system appgroup && \
    adduser --uid 2000 --system appuser --gid 2000

RUN mkdir -p /wiremock
WORKDIR /wiremock


COPY stubs /home/wiremock

RUN chown -R appuser:appgroup /wiremock


USER 200
