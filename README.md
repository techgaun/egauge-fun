# egauge-fun
Having fun with egauge - http://www.egauge.net/

### Hacking all egauge devices

Egauge identifiers seem to be just 4-5 digit code which means we could just iterate from 1000 to 100000 and run any of the calls that we can perform. Most likely, many of the endpoints can be called without authentication as its not uncommon for people to disable authentication.

### Undocumented endpoints

#### Get configuration parameters

Looks like this could be replayed to get other configuration parameters. Just need to figure what they could be.

```
http://<egauge_id>.egaug.es/cgi-bin/get?lang

# Other params:
installerURL
```

#### Get eGauge status

```
http://<egauge_id>.egaug.es/status.xml

# spits out egauge device status
```

#### Get eGauge configuration

```
http://egauge17984.egaug.es/cgi-bin/egauge-cfg?

# gives entire egauge configuration which is basically every kind of config
# quite revealing
```
