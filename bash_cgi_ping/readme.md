Note: this is not a beginner's guide! Knowledge of Apache, jQuery and bash is
almost certainly necessary.

The design comprises a bash CGI script to execute the actual ping and a an HTML
file with embedded jQuery to parse an external hosts file, generate the HTML and
periodically update the CSS depending on the ping result.

##CGI ping
The ping is handled via a bash CGI script and must be installed on a webserver within your subnet.
```
http://<server>/cgi-bin/ping?10.10.10.10
```

###Return values
- -1 - not an IP
- 0 - no response
- 1 - OK

Note use of `Access-Control-Allow-Origin: *` to allow calls from another server.

##HTML
The HTML is includes only the head and body tags, the hosts are rendered
on-the-fly using jQuery.

##jQuery
The jQuery script fetches the hosts file, extracts the uncommented IPs, renders
the HTML and the updates the CSS.
