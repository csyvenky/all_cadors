# all_cadors Splunk App
Splunk App to process Transport Canada Aviation Safety Data

*This is a work in progress.*

# Setup
1. Create an index on your Splunk instance, I called mine "*flight_aware_dump*".
2. Head over to the PiAware project and setup forwarder to send some [JSON data](https://flightaware.com/adsb/piaware/).
3. Point your forwarder's inputs.conf to the /run/dump1090-fa/*.json path; set "*flight_aware_dump*" as the sourcetype and index.
4. Install the app.

# Install
1. Navigate to $SPLUNK_HOME/etc/apps
2. Execute: `git clone https://github.com/csyvenky/pi_aware.git`
3. Restart Splunk: via Splunk Web or any other way you know how.

# Use
1. Access the main [Dashboard](http://your-splunk-ip:8000/en-US/app/flightaware/piaware)