Experitest - Audio Service ansible role for Cloud Agent
=========

This role will install audio service on cloud agent for mac os hosts. It support Mac Mojave distribution 10.14 currently.

Requirements
------------

* [ansible-role-java8](https://github.com/ExperitestOfficial/ansible-role-java8) must be installed on all machines. <br>
* Cloud Agent should be installed on mac with version 12.7 or above to {installation_root_folder} <br>
* Supports mac os hosts only, distribution 10.14 or above <br>
* Required audio input to be connected prior to the installation, UI approval during first installation (of each USB input device) and audio service restart afterwards <br>
* The service that will require reload will be situated in ~/Library/LaunchAgents/com.experitest.audiosupport.plist <br>
* Service reload is also required after every audio input device connection <br>

Role Variables
--------------

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| state | should the application be present or absent | present, absent | present | no |
| installation_root_folder | the root folder in which the audio service will be installed under audiosupport folder | string | for mac: /Applications/Experitest | no |
| autologin_pass | password for auto login | strings |  | yes |


Example Playbook
----------------

#### [see working example](/example)
