#	Leveling Up with SQL

Mark Simon이 집필한 《Leveling Up with SQL》(Apress, 2023)의 보조 자료 저장소입니다.

[comment]: #cover
![Cover image](978-1-4842-9684-4.jpg)

버전 v1.0은 출간된 책에 포함된 코드와 동일하며, 수정이나 업데이트는 포함되어 있지 않습니다.

-	[Downloading the Sample Database](#sample-database)
-	[The Exercise Files](#exercise-files)

##	샘플 데이터베이스 다운로드

예제들을 따라 해보려면 샘플 데이터베이스를 설치해야 합니다. 샘플 데이터베이스를 얻는 방법은 세 가지가 있습니다:

-	[정적(Static) 스크립트 파일 다운로드](#static-script-files)

	이 저장소에 저장되어있는 샘플 스크립트 파일 모음입니다.

-	[동적(Dynamic) 스크립트 파일 다운로드](#dynamic-script-files)

	다양한 연습을 해볼 수 있도록 무작위로 생성된 샘플 데이터를 포함한 스크립트입니다.

-	[샘플 데이터베이스 사이트 방문하기](#sample-database-site)

	다양한 옵션을 선택해 샘플 데이터베이스 스크립트를 생성할 수 있습니다.

세 가지 방법 모두 기본적으로 동일한 데이터베이스 구조를 제공합니다. 차이점이 있다면 실제 데이터 값이 고정되어 있는지, 무작위로 생성되는지 입니다.

###	스크립트 사용법

1.	데이터베이스 클라이언트를 통해 새 데이터베이스를 생성합니다. 이름은 __bookworks__ 와 같이 설정하면 됩니다.

2.	앞서 다운로드한 스크립트 파일을 열어 새로 만든 데이터베이스에 실행합니다.

###	정적(Static) 스크립트 파일

사용 중인 DBMS에 맞는 스크립트 파일을 받으면 쉽게 데이터베이스를 준비할 수 있습니다.

-	[PostgreSQL](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-pgsql-10-script.sql)
-	[SQLite](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-sqlite-script-script.sql)
-	[MySQL/MariaDB](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-mysql-mariadb-ansi-script.sql)
-	[Microsoft SQL](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-mssql-16-script.sql)
-	Oracle
	-	[Oracle (Plain)](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-oracle-12-script.sql)
	-	[Oracle (SQL Plus)](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-oracle-12-plus-script.sql)

만약 데이터를 좀 더 다양하게 다루고 싶다면, 동적(Dynamic) 스크립트 파일을 사용하는 것도 좋은 방법입니다.

###	동적(Dynamic) Script Files

The following links will generate database script files similar to the static script files above.

The difference is that the dynamic scripts will have different content every time you download.

-	PostgreSQL

	-	[PostgreSQL from version 10](https://sample-db.net/?dbmss[]=pgsql-10&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)

-	SQLite

	-	[SQLite Script plus File](https://sample-db.net/?dbmss[]=sqlite-script&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)

	-	[Database File Only](https://sample-db.net/?dbmss[]=sqlite-file&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)

-	MySQL / MariaDB

	-	[MySQL / MariaDB File (ANSI Mode)](https://sample-db.net/?dbmss[]=mysql-ansi&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)

	-	[MySQL / MariaDB File (Traditional Mode)](https://sample-db.net/?dbmss[]=mysql-traditional&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)

-	Microsoft SQL

	-	[MSSQL from version 2016](https://sample-db.net/?dbmss[]=mssql-16&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)
	-	[MSSQL up to version 2014](https://sample-db.net/?dbmss[]=mssql-14&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)

-	Oracle

	-	[From version 12c (Plain)](https://sample-db.net/?dbmss[]=oracle-12&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)
	-	[From version 23c (Plain)](https://sample-db.net/?dbmss[]=oracle-23c&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)
	-	[From version 12c (SQLPlus)](https://sample-db.net/?dbmss[]=oracle-12-plus&dbmss[]=oracle-23c&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)
	-	[From version 23c (SQLPlus)](https://sample-db.net/?dbmss[]=oracle-23c-plus&db=books&br=crlf&refresh&extra-tables[]=towns&extra-tables[]=countries&exercises)

This will download a freshly randomised script for current versions of you preferred DBMS.

If you want to download more than one script, or you want to vary the options, read the next section.

###	Sample Database Site

[https://www.sample-db.net/](https://www.sample-db.net/)

The full download page looks like this:

<img src="images/sample-db.png" alt="Sample DB Site" width="50%">

This will download a script to generate the sample database. The sample is re-generated every time with random values.

Choose the following options:

1.	Choose a refresh date. The sample sales data will be calculated up to this date.

	You can leave this at the default.

2.	Select the Sample Database

	For this book the sample is expected to be called __bookworks__.

3.	Select the DBMS

	You can choose more than one if you like.

	For Oracle, there are some quirks in the script which may not be understood by your particular client. You can try both scripts and see which one doesn’t have any errors.

4.	Select the Additional `Towns` and `Countries` tables.

5.	The Exercise file includes the sample SQL code from the book.

6.	Select the Line Break

	If you’re doing this on macOS or Linux, the standard line break is the __LF__ character. On Windows, you use the __CRLF__ combination. However, it probably doesn’t matter in most clients.

7.	Click on the generated __Download__ link.

	If you select a single database script, it will be downloaded as a single file with the `.sql` extension. If you choose more than one database file, they will be packaged in Zip file.

##	Exercise Files

The SQL samples in the text are there for you try on your database client. They have also been gathered in single sql files for your convenience:

-	[PostgreSQL](https://github.com/Apress/leveling-up-sql/blob/master/exercise-files/postgresql.sql)
-	[SQLite](https://github.com/Apress/leveling-up-sql/blob/master/exercise-files/sqlite.sql)
-	[MySQL/MariaDB](https://github.com/Apress/leveling-up-sql/blob/master/exercise-files/mysql-mariadb.sql)
-	[Microsoft SQL](https://github.com/Apress/leveling-up-sql/blob/master/exercise-files/mssql.sql)
-	[Oracle](https://github.com/Apress/leveling-up-sql/blob/master/exercise-files/oracle.sql)





