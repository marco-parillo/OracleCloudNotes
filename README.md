# OracleCloudNotes

## Container exits

* [Hat-tip](https://www.reddit.com/r/oraclecloud/comments/uyv4b0/next_cloud_works_until_i_exit_my_ssh_session/).
* [Troubleshooting tip](https://github.com/containers/podman/blob/main/troubleshooting.md#17-rootless-containers-exit-once-the-user-session-exits).
```
loginctl enable-linger $UID
```
## Create a simple HTTPS server with OPENSSL S_SERVER
* [Hat-tip](https://superhero.ninja/2015/07/22/create-a-simple-https-server-with-openssl-s_server/).
* Run once:
```
openssl req -x509 -newkey rsa:2048 -keyout key.pem -out cert.pem -days 365 -nodes
```
* Start the OpenSSL s_server
```
openssl s_server -key key.pem -cert cert.pem -accept 44330 -www
```
* Accessing the s_server via web browser
```
https://localhost:44330
```
* Acceot the privacy warning
