WA KAT
=========

Get wa-kat from repo, builds docker image a run it.

Repository: https://github.com/webarchivcz/wa-kat
Documentataion: http://wa-kat.readthedocs.io/en/latest/

Example Playbook
----------------

```
 - name: Web archiving catalogization assistence as web service
   hosts: docker
   roles:
     - role: NLCR.wakat
       tags: wa-kat
       wa_kat:
         repo: /opt/git/wa-kat
         packages: present # present, absent, latest
         release: HEAD # HEAD for latest, for specific release: v1.1.8
         port: 8080
```
