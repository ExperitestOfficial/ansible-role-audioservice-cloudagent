Experitest - Audio Service ansible role for Cloud Agent
=========

This role will install audio service on cloud agent for mac os hosts. It support Mac Mojave distribution 10.14 currently.

Requirements
------------

This role assumes that you have java 8 installed on the instance <br>
Cloud Agent should be installed on mac with version 12.7 or above <br>
Supports mac os hosts only, distribution 10.14 or above


Role Variables
--------------

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| state | should the application be present or absent | present, absent | present | no |
| installation_folder | the folder in which the audio service will be installed | string | for mac: /Applications/Experitest/cloud-agent-version <br> for windows: C:\\Experitest\\cloud-agent-version  | no |


Example Playbook
----------------

#### [see working example](/example)
