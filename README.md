# imap_email_html_content
Custom implementation of the Home Assistant imap_email_content sensor that includes a "force_html:" option.

How to use:
- Download this repository zip
- Extract zip
- Move imap_email_html_content/imap_email_html_content folder to your Home Assitant custom_components folder. 
    - End result: config/custom_components/imap_email_html_content/sensor.py
- Setup config on Home Assitant config file

Example config:
```
sensor:
  - platform: imap_email_html_content
    name: Citi Card Transactions
    server: imap.gmail.com
    port: 993
    username: YOUR_USERNAME
    password: YOUR_PASSWORD
    folder: YOUR_FOLDER
    senders:
      - example@gmail.com
    force_html: true
```
