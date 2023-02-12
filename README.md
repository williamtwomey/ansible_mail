# ansible_mail

Populate the following sensitive files:

* opendkim txt/private files in files/mail/opendkim
* postfix maps in files/mail/sasl_passwd,relayhost_map,access,sender_access

Define the following required vars:
* mail_users: []
* mail_domains: []
* http_domains: []
* mail_default_domain: example.com

This also assumes where you're running ansible from is running certbot and has /etc/letsencrypt available.
