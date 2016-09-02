# jpa-run-sql
run .sql with jpa


```xml
   <properties>
    <property name="javax.persistence.jdbc.driver" value="org.postgresql.Driver"/>
    <property name="javax.persistence.jdbc.url"
              value="jdbc:postgresql://tstt05dock01:5432/common-rsql?stringtype=unspecified"/>
    <property name="javax.persistence.jdbc.user" value="postgres"/>
    <property name="javax.persistence.jdbc.password" value="postgres"/>
    <property name="hibernate.hbm2ddl.auto" value="create-drop"/>
    <property name="javax.persistence.schema-generation.create-source" value="metadata"/>
    <property name="javax.persistence.schema-generation.drop-source" value="metadata"/>
    <property name="javax.persistence.sql-load-script-source" value="META-INF/createFunction.sql"/>
  </properties>
```

```xml
|-resources
  |-META-INF
    |-createFunction.sql
    |-persistence.xml
  ```
