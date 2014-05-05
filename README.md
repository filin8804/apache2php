apache2php
==========

Ansible Package to provision apache and php

Create and configure VHosts
---------------------------

        # vars/main,yml
        vhost_sites:
          - {
          host: 'app.local',
          docroot: '/vagrant/web',
          admin_email: 'admin@app.local',
          aliases: [
              app.dev
              app.local.dev
            ]
          }
      
This creates a vhost without ssl, the document root set to /vagrant/web and several server aliases
