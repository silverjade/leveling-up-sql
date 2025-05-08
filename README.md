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

###	정적 스크립트 파일

사용 중인 DBMS에 맞는 스크립트 파일을 받으면 쉽게 데이터베이스를 준비할 수 있습니다.

-	[PostgreSQL](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-pgsql-10-script.sql)
-	[SQLite](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-sqlite-script-script.sql)
-	[MySQL/MariaDB](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-mysql-mariadb-ansi-script.sql)
-	[Microsoft SQL](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-mssql-16-script.sql)
-	Oracle
	-	[Oracle (Plain)](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-oracle-12-script.sql)
	-	[Oracle (SQL Plus)](https://github.com/Apress/getting-started-sql-databases/blob/master/static-scripts/books-oracle-12-plus-script.sql)

만약 데이터를 좀 더 다양하게 다루고 싶다면, 동적 스크립트 파일을 사용하는 것도 좋은 방법입니다.

###	동적 스크립트 파일

아래 링크들은 앞서 소개한 정적 스크립트 파일과 유사한 데이터베이스 스크립트를 생성해줍니다.
다만 동적 스크립트는 매번 다운로드할 때마다 내용이 달라진다는 차이점이 있습니다.

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

위 링크를 통해 각 DBMS에 맞는 무작위 샘플 데이터를 포함한 최신 스크립트를 받을 수 있습니다.

스크립트를 여러 개 다운로드하거나 다양한 설정을 바꾸고 싶다면 다음 섹션을 참고하세요.

###	샘플 데이터베이스 사이트

[https://www.sample-db.net/](https://www.sample-db.net/)

위 사이트의 전체 다운로드 페이지는 다음과 같습니다.

<img src="images/sample-db.png" alt="Sample DB Site" width="50%">

이곳에서 샘플 데이터베이스를 생성하는 SQL 스크립트를 다운로드할 수 있습니다.
샘플은 매번 다운로드 시 무작위 값으로 재생성됩니다.

설정방법

1.	데이터 생성 기준 날짜 선택
	샘플 매출 데이터는 이 날짜까지의 데이터를 기준으로 생성됩니다.
	기본값 그대로 두어도 무방합니다.

2.	샘플 데이터베이스 선택
	이 책에서는 데이터베이스 이름을 __bookworks__ 로 설정했습니다.

3.	DBMS 선택

	하나 이상의 DBMS를 선택할 수 있습니다.

	Oracle의 경우 클라이언트에 따라 일부 스크립트가 호환되지 않을 수 있으므로, 두 가지 형식(Plain, SQLPlus)을 모두 시도해보는 것이 좋습니다.

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





