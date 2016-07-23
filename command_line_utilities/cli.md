## ps
All processes
```
ps -e
```

Full
```
ps -f
```

Only process 32701
```
ps -32701
```

Command name
```
ps -C vi
```

SE context
```
ps --context
```

ASCII art process tree
```
ps --forest
```

Thread info
```
TBD
```

## top
- i - hide idle tasks
- r 19 - renice to lowest user priority

## iotop
Show disk accesses

## dd
Check progress of `dd` running in the background.
```
dd if=/dev/zero of=/dev/null& pid=$!
kill -USR1 $pid; sleep 1; kill $pid
```
## vmstat
```
sudo vmstat -m # slab
sudo vmstat -f # fork
sudo vmstat -d # disk 
sudo vmstat -s # stat 
```
## iostat
observing the time the devices are active  in  relation to their average transfer rates. 

## sar
TBD

## uptime
Load average is for the last one, five and fifteen minutes.
```
 15:24:44 up 6 days, 20:45,  4 users,  load average: 0.55, 0.87, 0.83
 ```

## ipcs
Show resource limits
```
ipcs -l
```

