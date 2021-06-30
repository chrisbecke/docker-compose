FROM openjdk:8

WORKDIR /app
ADD https://launcher.mojang.com/v1/objects/bb2b6b1aefcd70dfd1892149ac3a215f6c636b07/server.jar server.jar
COPY server/ .

CMD ["java", "-Xmx1024M", "-Xms1024M", "-jar", "server.jar", "nogui"]