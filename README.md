Apigee OPDK Setup Edge UI SAML Integration
=========

This role will integrate Edge UI with SAML using the Edge SSO component of the Apigee Edge platform.  


Requirements
------------

None.

Role Variables
--------------

| Variable Name | Description |
| --- | --- |
| edgeui_response_file_name | edge-ui-sample-response.conf |
| edgeui_response_file_path | "{{ opdk_installer_path }}/{{ edgeui_response_file_name }}" |
| edgeui_public_uris | http://{{ local_mgmt_ip }}:9000 |
| edgeui_sso_enabled | y |
| sso_public_url_port | 9099 |
| sso_public_url_scheme | http |
| sso_admin_name | ssoadmin |
| sso_admin_secret | Apigee123! |
| edgeui_sso_client_name | edgeui |
| edgeui_sso_client_secret | Apigee123! |
| edgeui_sso_client_overwrite | y |


Dependencies
------------

* apigee-opdk-modules

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: apigee-opdk-setup-edge-saml-config }

License
-------

Apache 2.0

Author Information
------------------

Carlos Frias



<!-- BEGIN Google Required Disclaimer -->

# Not Google Product Clause

This is not an officially supported Google product.
<!-- END Google Required Disclaimer -->
<!-- BEGIN Google How To Contribute -->
# How to Contribute

We'd love to accept your patches and contributions to this project. Please review our [guidelines](CONTRIBUTING.md).
<!-- END Google How To Contribute -->
