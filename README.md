[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://opensource.org/licenses/MIT)


# Check_MK AmuleDaemon

Description
-----------

Simple Check_MK local check for amule-daemon

Dependencies
------------
* `amulecmd` ([aMule Project](https://github.com/amule-project))
* `units` (Utility for converting amounts from one unit to another) 

Setup
-----

* `AMULED_CFG_FILE` 
  
  absolute /path/to/.aMule/remote.conf
  
* `AMULED_REMOTE_PASSWORD`

  your ECPassword used in `remote.conf`
  

Get agent directories and put script in LocalDirectory

```bash
$ /path/to/check_mk_agent | grep Directory
AgentDirectory: /etc/check-mk-agent
DataDirectory: /var/lib/check_mk_agent
SpoolDirectory: /var/lib/check_mk_agent/spool
PluginsDirectory: /usr/share/check-mk-agent/plugins
LocalDirectory: /usr/share/check-mk-agent/local
```