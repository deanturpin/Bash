Note: I haven't actually tried this on a webserver! (Until tomorrow...)

Simple bash CGI script to ping an IP. To be installed in the CGI bin on your
webserver. To be used with Javascript applications that need a ping.

##Usage
```
http://<server>/cgi-bin/ping?10.10.10.10
```

##Return values
- -1 - not an IP
- 0 - no response
- 1 - OK
