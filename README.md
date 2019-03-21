Metaverse Public Blockchain
=========

Metaverse(MVS) is a decentralised system based on the blockchain technology, through which, a network of smart properties, digital identities and value intermediators are established. 

https://github.com/mvs-org/metaverse

![Metaverse](https://github.com/mvs-org/metaverse/raw/master/doc/image/dev-path.jpg "Metaverse")

Requirements
------------

First working version on latest CentOS 7.3, should be also working fine with CentOS 7+

Role Variables
--------------

```
boost_work_dir: '/tmp/boost'
boost_version: '1.66.0'
boost_build_dir: 'boost_{{ boost_version.replace(".", "_") }}'
boost_tar_name: '{{ boost_build_dir }}.tar.bz2'
libbitcoin_work_dir: '/tmp/libbitcoin'
zeromq_work_dir: '/tmp/zeromq'
secp256k1_work_dir: '/tmp/secp256k1'
miniupnpc_work_dir: '/tmp/miniupnpc'
metaverse_work_dir: '/tmp/metaverse'
```

Dependencies
------------

Boost recipe is modified from https://github.com/toshitanian/ansible-boost
n/a

Example Playbook
----------------

After running 'ansible-galaxy install vorapoap.metaverse' as root
Create the playbook file (.yml) as follows:

---
- hosts: localhost
  user: root
  roles:
    - vorapoap.metaverse

License
-------

MIT

Author Information
------------------

[Vorapoap Lohwongwatana](https://www.linkedin.com/in/vorapoap/)
