# breathe-providence-beaco2n-site-status-script-v1

Breathe Providence maintains 25 low cost BEACO2N air sensors throughout the
city of Providence, Rhode Island. These sensors are capable of measuring NOx,
O3, CO, CO2, and PM2.5. All sensors also contain temperature and humidity
sensors for the purpose of calibration. The notebook provided
("status script.ipynb") downloads the most recent data from all 25 sensors
via the Beacon API in order to check their online status.

Note that a site's sensor must be offline for 6 hours in order to be considered
"offline" here.