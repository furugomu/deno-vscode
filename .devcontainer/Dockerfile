FROM buildpack-deps:scm

RUN set -ex; \
  apt-get update; \
  apt-get install -y --no-install-recommends \
    unzip \
  ; \
  rm -rf /var/lib/apt/lists/*

ENV DENO_INSTALL=/usr
ENV DENO_VERSION=1.0.0
RUN curl -fsSL https://deno.land/x/install/install.sh | sh -s v${DENO_VERSION}
