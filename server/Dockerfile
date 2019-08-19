FROM ewolff/docker-java
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
ADD litemall-all/target/litemall-all-0.1.0-exec.jar .
CMD /usr/bin/java -Xmx400m -Xms400m -jar litemall-all-0.1.0-exec.jar
EXPOSE 9091
