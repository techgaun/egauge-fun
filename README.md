# egauge-fun
Having fun with egauge - http://www.egauge.net/

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
