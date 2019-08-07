# DropboxSkillet
Skillet for securing Dropbox with the Palo Alto Networks Security Operating Platform

### Overview
Palo Alto Networks created Skillets to simplify the implementation of best practices associated with the Security 
Operating Platform.  This Skillet implements the configuration steps listed in the 
[Deployment Guide for Securing Dropbox](https://www.paloaltonetworks.com/resources/guides/securing-dropbox-deployment-guide).
This includes controls for the following Dropbox functions:
- Dropbox base
- Uploading of files
- Downloading of files
- File management controls such as renaming or creating files and folders
- Dropbox Paper application used for collaboration
- File commenting
- File sharing

The Skillet files are loaded into the Panhandler tool to provide a web interface to prompt for necessary input and run 
on a desired endpoint.  Please review the [Running Panhandler](https://panhandler.readthedocs.io/en/latest/running.html) 
guide for details on installing and starting Panhandler.

Please see [Installing Dropbox Skillet](docs/install.md) and [Using Dropbox Skillet](docs/usage.md) for instructions 
regarding this Skillet.

### Assumptions and Prerequisites

- Access to the [Panhandler](https://panhandler.readthedocs.io/en/latest/) tool.
- The PAN-OS and Panorama versions tested with this Skillet are 8.1 and 9.0.
- Firewalls must be operational. This Skillet only covers the policy specific to Dropbox and not the
deployment of the firewalls.
- DNS resolution is a requirement for the Dropbox rules to function correctly and is expected to be configured.
- For optimal results SSL Decryption should be configured.