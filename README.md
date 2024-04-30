# 📕 Proxmox Ubuntu VM

This repository contains an automation script and templates for deploying Ubuntu Server on Proxmox using Cloud-Init.

## Design goals

The objective is to utilise the provided automation script for deploying Ubuntu Server on Proxmox using Cloud-Init. This approach is necessary due to the absence of GitLab CI/CD with Terraform setup to create Proxmox virtual machines. By leveraging the automation script, we aim to streamline the deployment process and ensure consistent provisioning of Ubuntu Server instances on the Proxmox infrastructure.

## 🚀 Deployment Steps

1. First login to your Proxmox VE host terminal:
2. `git` this repository.
3. Go to the cloned folder.

### Preparing Cloud-Init Templates

1. Go to preparing-cloud-init-template folder.
2. Modify the `preparing-cloud-init-template` environment variables in the .env file according to your requirements.

```console
chmod +x create-template.sh
./create-template.sh
```

### Deploy DevBox with Cloud Init 

1. Go to deploy-with-cloud-init folder.
2. Modify the `deploy-with-cloud-init` environment variables in the .env file according to your requirements.
3. Modify the `vm-cloud-init.yaml` file according to your requirements.

```console
chmod +x deploy-vm.sh
./deploy-vm.sh
```

## 🔨🔧 Customization
Feel free to modify the deployment script and Cloud-Init template to suit your specific requirements. You can add additional configurations, modify network settings, or adjust any other parameters as needed.

## 🔎 Troubleshooting
If you encounter any issues during the deployment process or while configuring the Cloud-Init template, refer to the Proxmox and Cloud-Init documentation for troubleshooting guidance. You can also check the Proxmox host's log files for any relevant error messages.

## ❗ Disclaimer
This automation script and template are provided as-is and without warranty. Use them at your own risk. Make sure to thoroughly test the deployment in a non-production environment before deploying to production.

## 📄 License

MIT / BSD

## 🇬🇧🇭🇰 Author Information

* Author: Jody WAN
* Linkedin: https://www.linkedin.com/in/jodywan/
* Website: https://www.jodywan.com
