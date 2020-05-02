## ALERT! This is NOT FOR PRODUCTION, all risk will on your own!

This repository forks from [MariaDB server](https://mariadb.org)


# The motivation

During the time of coronavirus madness, I practice producing high performance index for SQL optimization. As we all well know, MariaDB forks from MySQL server by core members of the original MySQL team. I know MySQL long before, for me, at least, I realize MariaDB does not hold a strong personality which comparing to MySQL. So I start this project to make MariaDB takes other characteristic.


# The difference

So far, this repository has been modified the original MariaDB with:
* Configuration file my.cnf renamed to mariadb.conf
* Add the etc sub-directory under installation root as configuration file searching path
* Renamed some MySQL environment variables by replacing MYSQL with MARIADB in prefix, for example, MYSQL_HOME renamed to MARIADB_HOME

# What's next

The major and priority task is:

1. Remove MyISAM, because MariaDB has Aria(Mor Maria), which should be better than MyISAM
2. Replace InnoDB with XtraDB
