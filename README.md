# breathe-providence-beaco2n-site-status-script-v1

Breathe Providence maintains 25 low cost BEACO2N air sensors throughout the
city of Providence, Rhode Island. These sensors are capable of measuring NOx,
O3, CO, CO2, and PM2.5. All sensors also contain temperature and humidity
sensors for the purpose of calibration. The notebook provided
("status script.ipynb") downloads the most recent data from all 25 sensors
via the Beacon API in order to check their online status.

Note that a site's sensor must be offline for 6 hours in order to be considered
"offline" here. Additionally, this notebook pulls based on the current eastern
time zone time (either EST or DST). This is used when defining inputs to the API
as the Beacon API accepts PST as input. All *outputs* of the API use UTC,
including the plots.