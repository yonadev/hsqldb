FROM java:8

WORKDIR /opt/hsqldb

EXPOSE 9001

RUN wget http://sourceforge.net/projects/hsqldb/files/hsqldb/hsqldb_2_3/hsqldb-2.3.2.zip && unzip hsqldb-2.3.2.zip
ENTRYPOINT ["java", "-cp", "hsqldb-2.3.2/hsqldb/lib/sqltool.jar", "org.hsqldb.Server", "-database.0", "file:thedatabase", "-dbname.0", "xdb"]
