# 基础镜像
FROM eclipse-temurin:17-jre-alpine
# 设定时区
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
# 拷贝jar包
COPY trade-service.jar /app.jar
# 入口
ENTRYPOINT ["java", "-Xms256m", "-Xmx512m", "-XX:MetaspaceSize=64m", "-jar", "/app.jar"]
