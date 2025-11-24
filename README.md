# Zabbix-ISC-Kea-Monitor

## What's this for?
This is for monitoring a ISC Kea DHCP cluster. This template is focussed around a hot-standby 2 node HA cluster. This will probably not work on more than a 2 node cluster. It also monitors the Kea API and has a few redundant alert triggers which may be helpful for as an early warning to an issue if the other trigger doesn't catch the certain scenario.

## Macro's
There's only one Macro. `{$KEACTRLPORT}` This port is set in your config. By default this macro is set port 8005

## Data collection Items:
<img width="1796" height="453" alt="image" src="https://github.com/user-attachments/assets/a83ee2d7-b41c-4b59-bfda-d1d1f455ebc4" />

## Triggers
<img width="1814" height="362" alt="image" src="https://github.com/user-attachments/assets/cd705158-8f46-493b-abfd-a0966c8f6b48" />

## Web Scenarios
The API Monitor is done via a Web Scenario. It expects HTTP 200 response. The trigger for the Web Scenario can be seen above.
