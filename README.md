# README

## Assumptions:
- Each system uses a distro with apt.
- I can use the rbenv role to install ruby 2.2.3 (ansible-galaxy install zzet.rbenv)
- Each worker is on a different server but they are the same type of worker (sidekiq) setup, just two different servers.
- We are going to send all logs to the remote server, and then filter out based on a tag.
- I just copied the rsyslog.conf off my linux system (Linux Mint 16) figuring that would work for this purpose.

## Resources Used:
- http://docs.ansible.com/ansible/
- https://github.com/ansible/ansible-examples
- https://galaxy.ansible.com/list#/roles/102
- https://github.com/crushlovely/ansible-sidekiq-upstart For a look at how to install/start sidekiq
- https://vexxhost.com/resources/tutorials/how-to-setup-remote-system-logging-with-rsyslog-on-ubuntu-14-04-lts/
- https://github.com/mperham/sidekiq/wiki/Logging
- http://askubuntu.com/questions/318852/rsyslog-filter-by-tag
