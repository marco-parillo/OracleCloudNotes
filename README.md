# OracleCloudNotes

## Container exits

* [Hat-tip](https://www.reddit.com/r/oraclecloud/comments/uyv4b0/next_cloud_works_until_i_exit_my_ssh_session/).
* [Troubleshooting tip](https://github.com/containers/podman/blob/main/troubleshooting.md#17-rootless-containers-exit-once-the-user-session-exits).
```
loginctl enable-linger $UID
```
