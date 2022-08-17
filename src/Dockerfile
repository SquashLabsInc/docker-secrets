# syntax=docker/dockerfile:1.2
FROM python:3.6.1-onbuild

COPY . /usr/src/app
# shows secret from default secret location:
RUN --mount=type=secret,id=sqenv cat /run/secrets/sqenv

CMD ["bash", "run_server.sh"]
