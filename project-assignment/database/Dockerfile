FROM postgres:15-alpine

ENV POSTGRES_DB=appdb
ENV POSTGRES_USER=appuser
ENV POSTGRES_PASSWORD=apppass

RUN mkdir -p /custom-init

HEALTHCHECK --interval=10s --timeout=5s --retries=5 \
  CMD pg_isready -U ${POSTGRES_USER} -d ${POSTGRES_DB} || exit 1
