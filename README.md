# Crystal Multi-tool

Crystal Multi-Tool (CMT) is an Ansible Playbook for installing X-ray crystallography sofware suites. Each suite is installed through an Ansible role.

CMT and it's roles are written for CentOS 7.

# In development!

This software is not yet complete. Currently the CCP4, Coot, and XDS roles are useful. DIALS and PHENIX will be added soon.

## CMT Suites

| Suite                                                         | Primary use                        |
|---------------------------------------------------------------|------------------------------------|
| [ccp4](http://www.ccp4.ac.uk/tutorials/targets/standard/)     | Crystal data refinement            |
| [Coot](https://www2.mrc-lmb.cam.ac.uk/personal/pemsley/coot/) | Crystal data real-space refinement |
| [DIALS](https://dials.github.io/)                             | Crystal data processing            |
| [PHENIX](https://www.phenix-online.org/)                      | Crystal data refinement            |
| [Rosetta](https://www.rosettacommons.org/software)            | Molecular replacement              |
| [XDS](http://xds.mpimf-heidelberg.mpg.de/)                    | Crystal data processing            |

## Using CMT

Download the following roles to the `roles/` folder of CMT:
 - [os](https://github.com/crystal-multi-tool/os.git)
 - [ccp4](https://github.com/crystal-multi-tool/ccp4.git)
 - [coot](https://github.com/crystal-multi-tool/coot.git)
 - [dials](https://github.com/crystal-multi-tool/dials.git)
 - [phenix](https://github.com/crystal-multi-tool/phenix.git)
 - [rosetta](https://github.com/crystal-multi-tool/rosetta.git)
 - [xds](https://github.com/crystal-multi-tool/xds.git)

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
