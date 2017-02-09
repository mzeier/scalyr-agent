# Scalyr Agent

This role installs and configures the Scalyr logging agent. See [https://www.scalyr.com/](https://www.scalyr.com/).

The role was inspired from the "[Install Scalyr Agent (Linux)](https://www.scalyr.com/help/install-agent-linux#install)" documentation.

## Requirements
You will need an account with Scalry with a Write API key.

## Role Variables
Variable | Description |
-----|-----------------|
`scalyr_api_key`|Your Scalyr Write API key

## Example Playbook
    --- 
    - hosts: all
    - roles:
       - { role mzeier.scalyr, scalyr_api_key: '0/kjoau98098123' }