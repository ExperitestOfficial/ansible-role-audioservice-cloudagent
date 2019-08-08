Experitest - Audio Service ansible role for Cloud Agent
=========

This role will install audio service on cloud agent for mac os hosts. It support Mac Mojave distribution 10.14 currently.

Requirements
------------

This role assumes that you have java 8 installed on the instance <br>
Cloud Agent should be installed on mac with version 12.7 or above <br>
Supports mac os hosts only, distribution 10.14 or above <br>
Required audio input to be connected prior to the installation, UI approval during installation and audio service restart afterwards <br>
The service that will require reload will be situated in ~/Library/LaunchAgents/com.experitest.audiosupport.plist <br>
Service reload is also required after every audio input device connection <br>

Role Variables
--------------

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| state | should the application be present or absent | present, absent | present | no |
| installation_folder | the folder in which the audio service will be installed | string | for mac: /Applications/Experitest/cloud-agent-version <br> for windows: C:\\Experitest\\cloud-agent-version  | no |
| autologin_pass | password for auto login | strings |  | yes |


Example Playbook
----------------

#### [see working example](/example)
