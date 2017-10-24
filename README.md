
Docker Pure-ftpd Server


build
------------------------------
docker build --rm -t mylinftp .
------------------------------


run
------------------------------------------

docker run -d --name ftplin -p 21:21 -p 30000-30009:30000-30009 -e "PUBLICHOST=localhost" mylinftp

------------------------------------------


test
-------------------------------
ftp -p loclhost 21
-------------------------------
