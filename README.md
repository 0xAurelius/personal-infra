# personal-infra

# Initial one-time setup

- Create GCP account
- Create service account: https://console.cloud.google.com/iam-admin/serviceaccounts
- Create a JSON key for the service account and place at {{ gcp_cred_file }}
- Add Compute Engine API to project: https://console.developers.google.com/apis/api/compute.googleapis.com/overview
- Configure an SSH key for the service account to enable OSLogin: https://alex.dzyoba.com/blog/gcp-ansible-service-account/

# Local workstation setup
- Download JSON credentials and set file location under gcp_cred_file or env variable
- Configure GCP_ environment variables for easier injection:
    - 
    - 
    - 
- Place SSH key into ~/.ssh folder and set permissions with `chmod 700 ...` 
- Install Ansible locally e.g. apt-get install ansible
- Install gcloud: 
- Install google-auth Python package via pip

# Run main playbook

```
ansible-playbook playbook.yml -i inventory/dev
```