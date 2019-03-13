FROM openjdk

COPY target/webapp-1.0-SNAPSHOT-jar-with-dependencies.jar /opt/webapp-1.0-SNAPSHOT-jar-with-dependencies.jar

CMD java -jar /opt/webapp-1.0-SNAPSHOT-jar-with-dependencies.jar

FROM couchbase:community-5.1.1

COPY configure.sh /opt/couchbase

CMD ["/opt/couchbase/configure.sh"]
