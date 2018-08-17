# all_cadors Splunk App
Splunk App to process Transport Canada Aviation Safety Data

*This is a work in progress.*

# Setup
1. Create an index on your Splunk instance, I called mine "*cadors_all*".
2. Head over to Transport Canada and get some [XML CADORS data](http://wwwapps.tc.gc.ca/saf-sec-sur/2/cadors-screaq/m.aspx?lang=eng).
3. Point your file input monitor at your data folder; select "*cadors_all*" as the sourcetype.
4. Install the app.

# Install
1. Navigate to $SPLUNK_HOME/etc/apps
2. Execute: `git clone https://github.com/csyvenky/all_cadors.git`
3. Restart Splunk: via Splunk Web or any other way you know how. Alternatively, you can use the Ansible Playbook 
*restart_splunk.yml* - a quick and dirty restart tool for splunkd.
    ```
    ansible-playbook -i hosts restart_splunk.yml --ask-pass
    ```

# Use
1. Access the [main Dashboard](http://&lt;your splunk&gt;:8000/en-GB/app/all_cadors/all_cadors_dashboard)