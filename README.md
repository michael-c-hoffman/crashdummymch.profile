Role Name
=========

Profile module for managing /etc/profile and /etc/profile.d/* profiles

Requirements
------------

None

Role Variables
--------------
  profile_profile_manage = bool manage /etc/profile or not
  profile_profile_path = string path to /etc/profile 
  profile_profiled_path = string path to directory to place profiled files
  profile_bashrc_manage = bool manage /etc/bashrc or not
  profile_bashrc_path = string path to system bashrc file
  profile_profiled_templates = list of templates to copy into /etc/profile.d
  profile_privilage_escalation = bool whether privilage escalation is needed
  profile_privilage_user = string user to privilage escalate to
  profile_owner = string owner to set files
  profile_group = string group to set files
  profile_mode = string mode to set files 
  profile_environment_path = string to environment path
  profile_environment_manage = bool manage /etc/environment or not

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: crashdummymch.profile }

License
-------

GPLv3
