# Adding and removing clients #

While the presence (or absence) of client update packets (see "Positon updates" under "Requesting and sending information") will signify the presence (or lack thereof) of a client, the server will also send a special packet signaling the addition/removal of said client, whether this is due to client disconnecting or falling out of visibility range.

The following commands are also used to login/logoff the client itself.



## Adding clients ##

It is unknown as to what `100` represents, but it appears that all clients share the same value.

### ATC ###

```
#AA(callsign):SERVER:(real name):(network ID)::(rating):(protocol version)
```

### Pilots ###

```
#AP(callsign):SERVER:(network ID)::1:(protocol version):(rating):(real name ICAO)
```



## Removing clients ##

### ATC ###

```
#DA(callsign):(network ID)
```

### Pilots ###

```
#DP(callsign):(network ID)
```



