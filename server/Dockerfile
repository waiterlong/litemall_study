FROM ewolff/docker-java
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
ADD litemall-all/target/litemall-all-0.1.0-exec.jar .
#ADD litemall-admin-api/target/litemall-admin-api-0.1.0.jar .
#ADD litemall-core/target/litemall-core-0.1.0.jar .
#ADD litemall-db/target/litemall-db-0.1.0.jar .
#ADD litemall-wx-api/target/litemall-wx-api-0.1.0.jar .
CMD /usr/bin/java -Xmx400m -Xms400m -jar litemall-all-0.1.0-exec.jar
EXPOSE 9091
