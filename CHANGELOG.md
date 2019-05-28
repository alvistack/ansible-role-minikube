# Ansible Role for Kubernetes

## 3.1.0 - TBC

### Major Changes

  - Always use `become: true` with molecule, especially for vagrant
  - Replace `inventory_hostname` with `ansible_hostname`

## 3.0.0 - 2019-05-20

### Major Changes

  - Upgrade minimal Ansible support to 2.8.0
  - Debug CNI for Flannel installation
  - Disable all addons by default

## 2.6.0 - 2019-05-04

### Major Changes

  - Refine Travis CI Molecue test cases

## 2.5.0 - 2019-04-30

  - Initial release for Ansible 2.6 or higher
  - Support both Ubuntu 16.04/18.04 or RHEL/CentOS 7 or openSUSE Leap 15
