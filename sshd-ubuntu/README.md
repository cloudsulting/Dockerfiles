Build
`docker build -t sshd_server .`

Run
`docker run -d -P --name test_sshd sshd_server`

Find port
`docker port test_sshd 22`
`# 0.0.0.0:32776`

Connect
`ssh root@localhost -p 32776`
`# password is root`
