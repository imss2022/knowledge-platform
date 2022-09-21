FROM sunbird/openjdk-java11-alpine:latest
COPY  ./schemas /workspace/source/assessment-api/assessment-actors/target/assessment-actors-1.0-SNAPSHOT.jar/schemas
CMD java -XX:+PrintFlagsFinal $JAVA_OPTIONS -cp '/workspace/source/assessment-api/assessment-actors/target/assessment-actors-1.0-SNAPSHOT.jar/lib/*' -Dconfig.file=/home/sunbird/assessment-service-1.0-SNAPSHOT/config/application.conf  -Dlogger.file=/home/sunbird/assessment-service-1.0-SNAPSHOT/config/logback.xml play.core.server.ProdServerStart /workspace/source/assessment-api/assessment-actors/target/assessment-actors-1.0-SNAPSHOT.jar
