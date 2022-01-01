# Ansible Crystallography Playbook

`ansible-crystallography` is a suite of Ansible roles for software tools used by crystallographers.

Each `ansible-crystallography` role installs a a different crystallography tool. This role installs all roles (by default).

CentOS 7 is supported.

## Roles installed

| Role | Crystallography Tool | Primary use |
|------|----------------------|-------------|
| [ansible-ccp4](https://github.com/ansible-crystallography/ansible-ccp4.git) | [ccp4](http://www.ccp4.ac.uk/tutorials/targets/standard/) | Crystal data refinement |
| [ansible-coot](https://github.com/ansible-crystallography/ansible-coot.git) | [Coot](https://www2.mrc-lmb.cam.ac.uk/personal/pemsley/coot/) | Crystal data real-space refinement |
| [ansible-dials](https://github.com/ansible-crystallography/ansible-dials.git) | [DIALS](https://dials.github.io/) | Crystal data processing |
| [ansible-phenix](https://github.com/ansible-crystallography/ansible-phenix.git) | [PHENIX](https://www.phenix-online.org/) | Crystal data refinement |
| [ansible-rosetta](https://github.com/ansible-crystallography/ansible-rosetta.git) | [Rosetta](https://www.rosettacommons.org/software) | Molecular replacement |
| [ansible-xds](https://github.com/ansible-crystallography/ansible-xds.git) | [XDS](http://xds.mpimf-heidelberg.mpg.de/) | Crystal data processing |

## Using CMT

Download the following roles to the `roles/` folder of CMT:
 - [os](https://github.com/ansible-crystallography/os.git)

## Vagrant

CMT can be installed to a virtual machine with vagrant.

```bash
vagrant up --provision
```

To use GUI tools access the VM with:
```bash
vagrant ssh -- -X
```

## v1.0 to do list

- [ ] Add alpha roles for:
  - [x] CCP4
  - [X] Coot
  - [ ] DIALS
  - [ ] PHENIX
  - [X] Rosetta
  - [x] XDS
  - [ ] OS role
    - [ ] Add graphical hardware acceleration drivers
