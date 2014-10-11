php-fpm-status-monitor
======================

Php fpm status monitor is a plugin for Carbon and Graphite Ecosystem.It's collect performance data of PHP-FPM and send to Graphite. The metrics includes 

metrics = {"accepted conn":"accepted_conn","listen queue":"listen_queue","max listen queue":"max_listen_queue","listen queue len":"listen_queue_len","idle processes":"idle_processes","active processes":"active_processes","total processes":"total_processes","max active processes":"max_active_processes","max children reached":"max_children_reached","slow requests":"slow_requests"}

It's also collect  Network IO,Disk Io , CPU Usage ,Mem Usage of target host.

How to run
python data-collect.py

Run at debug mode
python data-collect.py -debug

Requirments

Graphite
  run as Apache WSGI
Carbon
  start by bin/carbon-cache.py start  
