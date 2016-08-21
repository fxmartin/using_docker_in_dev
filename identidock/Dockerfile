FROM hypriot/rpi-python

RUN groupadd -r uwsgi && useradd -r -g uwsgi uwsgi
RUN sudo apt-get update && sudo apt-get install -y apt-utils
RUN sudo apt-get -y install \
    gcc \
    libpcre3 \
    libpcre3-dev
RUN pip install \ 
    Flask==0.10.1 \
    uWSGI==2.0.8

WORKDIR /app

COPY app /app

COPY cmd.sh /

EXPOSE 9090 9191

USER uwsgi

CMD ["/cmd.sh"]
