# ddnss-update
Python3 updatescript for [DDNSS dynDNS service](https://www.ddnss.de/)

## Installation

* `pip3 install -r requirements.txt`
* change HOSTNAME and APIKEY
* `chmod a+x ddnss-update`

## Execution

* `./ddnss-update`

## Regularly check if IP has changed

Add the following line to `crontab -e`
`*/5 *   *   *   *    /usr/local/bin/ddnss-update 2>&1 | /usr/bin/logger -t DynDNS`
