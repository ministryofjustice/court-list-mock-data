FROM rodolpheche/wiremock

RUN addgroup --gid 2000 --system appgroup && \
    adduser --uid 2000 --system appuser --gid 2000

RUN mkdir -p /app
WORKDIR /app


COPY stubs /home/wiremock

RUN chown -R appuser:appgroup /app


USER 200
