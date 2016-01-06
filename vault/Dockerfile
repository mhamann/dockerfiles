FROM alpine:latest

RUN  apk add --update curl \
  && curl -o vault.zip https://releases.hashicorp.com/vault/0.4.0/vault_0.4.0_linux_amd64.zip \
  && unzip vault.zip \
  && mv vault /usr/local/bin/ \
  && rm -f vault.zip \
  && apk del curl \
  && rm -rf /var/cache/apk/* /usr/local/src/*

EXPOSE 8200

ENTRYPOINT [ "vault" ]
CMD [ "server", "-dev" ]
