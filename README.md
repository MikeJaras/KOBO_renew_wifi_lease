# KOBO_renew_wifi_lease
Script to run udhcpc from Xcsoar tools menu on Kobo busybox. Will renew ip address lease so wifi stays connected.
Solves my problem when I have the Kobo to connect to ESP32 softAP wifi and lease time is set to two hours without possibility to change it. 
The script will run udhcpc in a loop with a sleep of 30 sec. When it runs it will do a dhcp renew.

Place in /mnt/onboard/XCSoarData/kobo/scripts

to use it, start wifi the normal way, then select AAA_wifi from the tools page.

note that the scripts must be executable but normally that is set by default.
