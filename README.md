# certbot_dns_cloudflare

Wrapper of `geerlingguy.certbot` to generate certificates using DNS challenges and Cloudflare.

## Example playbook

```yaml
---
- hosts: foo
  roles:
    - role: someone_stole_my_name.certbot_dns_cloudflare
      vars:
        certbot_cloudflare_api_token: xxxxx
        certbot_admin_email: foo@bar
        certbot_certs:
          - domains:
              - "*.foo.bar"
              - "foo.bar"
```
