FROM ewolff/docker-java
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
ADD target/taskdispatcherserver-0.0.1-SNAPSHOT.jar .
CMD /usr/bin/java -Xmx400m -Xms400m -jar taskdispatcherserver-0.0.1-SNAPSHOT.jar
EXPOSE 9091
