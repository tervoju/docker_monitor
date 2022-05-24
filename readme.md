
# docker container monitoring with prometheus and grafana

inspiration from here

https://adamtheautomator.com/grafana-docker/#Conclusion

tested on wsl2 win11

```
Distributor ID: Ubuntu
Description:    Ubuntu 20.04.4 LTS
Release:        20.04
Codename:       focal
```

/etc/docker/daemon.json 

{
        "metrics-addr" : "127.0.0.1:9323",
        "experimental" : true
}

# metric used 

in dashboard

engine_daemon_container_states_containers{}

as "stats"

