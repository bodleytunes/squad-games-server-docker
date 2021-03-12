# squad-games-server-docker
Building a squad server for Adamski


##### Notes 

* Downloads 16gb+ of mapdata so had to add a 40gb volume to the hetzner cloud server

`/mnt/bigdisk40`

* watch the permissions on the "squad-data" folder, docker needs to be able to r/w to it

Ports allowed in ufw:
```
root@ubuntu-adam-squad:/mnt/bigdisk40/docker/squad# ufw status
Status: active

To                         Action      From
--                         ------      ----
22/tcp                     ALLOW       Anywhere
7787                       ALLOW       Anywhere
21114                      ALLOW       Anywhere
27165                      ALLOW       Anywhere
7788                       ALLOW       Anywhere
27166                      ALLOW       Anywhere
22/tcp (v6)                ALLOW       Anywhere (v6)
7787 (v6)                  ALLOW       Anywhere (v6)
21114 (v6)                 ALLOW       Anywhere (v6)
27165 (v6)                 ALLOW       Anywhere (v6)
7788 (v6)                  ALLOW       Anywhere (v6)
27166 (v6)                 ALLOW       Anywhere (v6)

```
