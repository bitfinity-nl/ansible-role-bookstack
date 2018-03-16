# ansible-role-bookstack
Automate bookstack on ubuntu 16.04lts

## Overwritable variable(s)

### MySQL server default variable(s)
{{ MySQL_ROOT_ACCOUNT }}

{{ MySQL_ROOT_PASSWORD }}

### BookStack default veriable(s)

### Database details

{{ bst_dbhost }}

{{ bst_dbname }}

{{ bst_dbuser }}

{{ bst_dbpass }}

{{ bst_domain }}

{{ bst_dir }}

### General auth

{{ bst_auth_method }}

### LDAP settings
  
{{ bst_ldap_server }}
  
{{ bst_ldap_basedn }}
  
{{ bst_ldap_dn }}
  
{{ bst_ldap_pass }}
  
{{ bst_ldap_user_filter }}
  
{{ bst_ldap_version }}
  
### Mail settings
{{ bst_mail_driver }}

{{ bst_mail_host }}

{{ bst_mail_port }}

{{ bst_mail_username }}

{{ bst_mail_password }}

{{ bst_mail_encryption }}

## LDAP Exampe(s)
     bst_ldap_server          : ldap://172.16.2.11:389
     
     bst_ldap_basedn          : ou=vgg,dc=vgg,dc=local
     
     bst_ldap_dn              : svc_bookstack@vgg.local
     
     bst_ldap_pass            : Bookstack123!
     
     bst_ldap_user_filter     : (&(samaccountname=${user}))
     
     bst_ldap_email_attribute : mail

