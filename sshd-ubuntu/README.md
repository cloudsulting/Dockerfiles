docker build -t sshd_server .
docker run -d -P --name test_sshd sshd_server
docker port test_sshd 22
