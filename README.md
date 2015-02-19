Some days you just need a simple http server


In this case, I'm messing around with a web api where everything was returning true.
But I don't want web servers running locally with root privs all the time.

So,   I sat down to figure out how systemd does the socket activation, and built in that.

Working example of doing http socket handover from systemd => python.

systemd-test is a simple "set environment and mess around" that spawns httpd-true.

