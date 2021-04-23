# sshd

sshd with logging to syslog on host (works with docker-fail2ban)

Inspiration for this container image was taken from panubo/docker-sshd.

I've added in logging via syslog, to a logfile held in a volume. In this way the Host machine can monitor the logfile.

Or as I have it deployed, where I use separate fail2ban container to monitor the logfile for nefarious behavior and manage the host firewall configuration accordingly.
