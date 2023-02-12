# ansible_mail

This playbook will setup a mail server with:

* postfix
* dovecot
* opendkim
* solr
* httpd/roundcubemail

Generate and put the following sensitive files into place:

* opendkim txt/private files for each domain in /files/openskim/domain.{txt,private}
* postfix maps in /files/ - sasl_passwd, relayhost_map, access, sender_access

Define the following required vars:
* mail_users: []
* mail_domains: []
* http_domains: []
* mail_default_domain: example.com

This assumes where you're running ansible from is running certbot and has /etc/letsencrypt available.
