Simple bash CGI script to ping an IP. To be installed in the CGI bin on your
webserver and used with Javascript applications that require a ping.

##Usage
```
http://<server>/cgi-bin/ping?10.10.10.10
```

##Return values
- -1 - not an IP
- 0 - no response
- 1 - OK

Note use of `Access-Control-Allow-Origin: *` to allow calls from another server.
