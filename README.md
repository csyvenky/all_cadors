# all_cadors Splunk App
Splunk App to process Transport Canada Aviation Safety Data

*This is a work in progress.*

# Install
1. Navigate to $SPLUNK_HOME/etc/apps
2. Execute: `git clone https://github.com/csyvenky/all_cadors.git`
3. Restart Splunk: via Splunk Web or any other way you know how. Alternatively, you can use the Ansible Playbook 
*restart_splunk.yml* - a quick and dirty restart tool for splunkd.
    ```
    ansible-playbook -i hosts restart_splunk.yml --ask-pass
    ```