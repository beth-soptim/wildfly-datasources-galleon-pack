Galleon Layers
=========

* `awswrapper-driver`: Provision the `aws-wrapper` driver. This layer installs the JBoss Modules module `software.amazon.jdbc`.

Configuration
========

The following set of environment variables and corresponding Java system properties can be used to configure the datasource.

Using plugins (https://github.com/aws/aws-advanced-jdbc-wrapper/blob/main/docs/using-the-jdbc-driver/UsingTheJdbcDriver.md#list-of-available-plugins) that require additional dependencieys is currently not supported.

Required configuration
==============

When using PostgreSQL the `POSTGRESQL_URL` must be set to include the `aws-wrapper` as driver name :`jdbc:aws-wrapper:postgresql://${POSTGRESQL_HOST}:${POSTGRESQL_PORT}/${POSTGRESQL_DATABASE}`

When using MySQL the `MYSQL_URL` must be set to include the `aws-wrapper` as driver name :`jdbc:mysql://${MYSQL_HOST}:${MYSQL_PORT}/${MYSQL_DATABASE}`

Optional configuration
==============

See https://github.com/aws/aws-advanced-jdbc-wrapper.

