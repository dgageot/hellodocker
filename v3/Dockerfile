FROM dgageot/maven

ENV PROD_MODE true
WORKDIR /home/jug
EXPOSE 8080
CMD java -server -DPROD_MODE=${PROD_MODE} -jar target/jug.jar

ADD . /home/jug
RUN mvn verify dependency:copy-dependencies -DskipTests
