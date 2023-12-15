FROM praqma/native-buck

WORKDIR /usr/src/myant

COPY bin .

RUN buck fetch :

# Add docker-compose-wait tool -------------------
ENV WAIT_VERSION 2.7.2

ADD https://github.com/ufoscout/docker-compose-wait/releases/download/$WAIT_VERSION/wait /wait

RUN chmod +x /wait

# CMD ["buck run :"
