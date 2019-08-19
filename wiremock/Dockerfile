FROM rodolpheche/wiremock

RUN addgroup -g 1000 -S appgroup && \
    adduser -u 1000 -S appuser -G appgroup


WORKDIR /wiremock

COPY stubs /home/wiremock

RUN chown -R appuser:appgroup /wiremock


USER 1000
