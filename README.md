💾 NodeJS script for obtaining public information about SA-MP server.

## Usage
>#### Get all info about server
```javascript
getServerInfo("127.0.0.1", 7777, function(error, response)
{
    console.log(response);
});
```
Instead of IP, you can also use the URL. As example `server.sa-mp.com`.
>#### Sample response
```
{
  passworded: false,
  players: 1,
  maxplayers: 10,
  servername: 'SA-MP Unofficial server',
  gamemodename: 'freeroam',
  language: 'English',
  property:
  { 
     artwork: 'Yes',
     lagcomp: 'On',
     mapname: 'San Andreas',
     version: '0.3.DL-R1',
     weather: '7',
     weburl: 'sa-mp.com',
     worldtime: '00:00' 
  },
  playerlist:
  [
      { id: 0, name: 'ufteers', score: 1, ping: 11 }
  ]
}
```
>#### Other functions
```javascript
getServerOnline(...)
getServerMaxPlayers(...)
getServerName(...)
getServerGamemodeName(...)
getServerLanguage(...)
getServerVersion(...)
getServerWeather(...)
getServerWebSite(...)
getServerWorldTime(...)
getServerPlayers(...)
```

## Soon
- [ ] Add support for cyrillic letters in texts
