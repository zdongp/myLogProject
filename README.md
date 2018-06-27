# myLogProject
Update system log by custom driver, use klogctl() to get the log and save to specified log file.

This is the project which update the log by custom driver and read the log to mylog.log.
When mylog.log size is more than 1k bytes, recover from the begining.
Documents include:
README, Chart_log_driver.pdf, bin, include, logmodule, src

Execution steps:
1.xxx# insmod logmodule.ko
2.xxx# mknod /dev/logdev c 520 0
3.xxx# ./readlog
4.xxx# ./logtest
