# Ansible role 'ansible-role-nfs-server'

An Ansible role for setting up an NFS server. Largely a reboot of Jeff Geerling's role to fit my other roles. 

## Requirements
One of the following distributions:
- RedHat Family
- Ubuntu 17+

Earlier releases of mentioned distributions might work, but no guarantees. Feel free to come with input.

## Role Variables
| Variable                       | Default                          | Comments (type)  |
| :---                           | :---                             | :---             |

## Dependencies

## Example Playbook
```Yaml
- hosts: foo
  roles:
    - role: ansible-role-nfs-server
      tags: nfs
      nfs_exports:
        - "/srv/nfs/ *(fsid=0,rw,sync,no_subtree_check)"
```

## Testing

## License

BSD

## Contributors

Issues, feature requests, ideas, suggestions, etc. are appreciated and can be posted in the Issues section. Pull requests are also very welcome. Please create a topic branch for your proposed changes, it's the easiest way to merge back into the project.

- [Oscar Petersson](https://github.com/oscpe262/) (Maintainer)
- [Geff Geerling](https://www.jeffgeerling.com) (Original role)
