FROM python:3.6
LABEL maintainer 'Juracy Filho <juracy at gmail.com>'
RUN useradd www && \
  mkdir /app && \
  mkdir /log && \
  chown www /log
USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000
ENTRYPOINT ["/usr/local/bin/python"]
CMD ["run.py"]

# docker build -t ex-build-dev .
# docker run -it -v $(pwd):/app -p 80:8000 ex-build-dev # Serviço disponível em http://localhost:80