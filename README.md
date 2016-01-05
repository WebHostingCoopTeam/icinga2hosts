# icinga2hosts


add .conf files to this [repo](https://github.com/WebHostingCoopTeam/icinga2hosts)

docs [here](http://docs.icinga.org/icinga2/latest/doc/module/icinga2/toc#!/icinga2/latest/doc/module/icinga2/chapter/monitoring-basics#hosts-services)

when you've added a host you can log into vigilante.whc and incant this:

```
 /root/refreshIcinga.sh
```

icinga will be rebuilt with your config in place, it will die if you gave it a bad conf file, in which case:

```
cd /exports/git/docker-icinga2/
```

then `make logs` will tell you most likely what happened, if not try `make enter` and look at supervisors logs `/var/log/supervisor` and also icingaweb2 `/var/log/icingaweb2`
