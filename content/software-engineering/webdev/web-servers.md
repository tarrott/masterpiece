---
title: "Web Servers"
date: 2021-01-31T18:46:49-05:00
draft: false
---

## nginx
- `nginx -t`: test config files


### Basic Auth
1. Install Apache tool to get access to the `htpassword` command: `apt-get install apache2-utils`
2. Run interactive prompt to create password for `<USER>`: `htpasswd -c /etc/nginx/.htpasswd <USER>`
    - Verify by taking a look at the file created: `vi /etc/nginx/,htpasswd`
3. Add basic auth directives (`auth_basic` & `auth_basic_user_file`) to appropriate nginx conf file: `vi /etc/nginx/sites-available/default.conf`
4. Reload nginx `service nginx reload`
