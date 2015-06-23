docker-openvpn
==============
Fork of cpuguy83's openvpn image using stronger crypto.

Pass "--udp" or "--tcp" into the docker run command to get the individual services.<br />
Default is "--udp"

This image requires NET_ADMIN and MKNOD capabilties.

```$ docker run -d -p 443:443 -p 1194:1194 --cap-add NET_ADMIN --cap-add MKNOD ewindisch/openvpn```

# To get the openvpn config to use, run:
docker exec <container> run --config
```



