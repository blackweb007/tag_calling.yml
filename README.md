# tag_calling.yml
---
- name
  hosts: all
  tasks:
    - name: Print Message one
      debug:
        msg: "write anything:{{anisble_user_gid}}"
      tags: tagone
    - name: Print Message two
      debug:
        msg: "write anything:{{ansible_env.LOGNAME}}"
      tags: tagtwo
...
