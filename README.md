# ansible_mail

Populate the following secrets:

* files/mail/opendkim -> with your opendkim .txt and .private files
* files/mail/sasl_passwd -> relay creds

Define mail_users, mail_domains and http_domains in host/group vars

This assumes where you're running ansible from is running certbot and has /etc/letsencrypt available.
