ECGALAXY ca_certificates role
========

Installs the ca-certificates package and adds certificates to the list of trusted CAs.

By default [CommisSign-2 CA certificates](https://commissign.pki.ec.europa.eu/index_en.htm)
are downloaded and added to the list.

Requirements
------------

The distribution-specific command to update CA certificates (see vars folder),
which should be available on most systems.

Role Variables
--------------

- `ca_certificates_download`: The list of certificates to add (default: CommisSign-2 certificates)

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.ca_certificates

One-liner
---------

    bash <(curl -s https://code.europa.eu/-/snippets/1/raw/main/ansible-role.sh) ecgalaxy.ca_certificates

See [ansible-role](https://code.europa.eu/-/snippets/1) for instructions.

Please verify the script integrity first.

License
-------

Copyright the European Union 2023.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

[ECGALAXY](https://code.europa.eu/groups/ecgalaxy/-/wikis/home) team.
