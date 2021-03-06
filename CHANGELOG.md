# Ansible Role for minikube

## 4.2.7 - 2020-04-03

### Major Changes

  - \[DEPRECATED\] No CRI-O support with `--vm-driver=none`, use kube\_master instead
  - Upgrade minimal Molecule support to 3.0.2
  - Migrate role name to lowercase or underline
  - Migrate group name to lowercase or underline
  - Migrate molecule `group_vars` to file
  - Consolidate molecule tests into `default` (noop)
  - Download archives to `{{ ansible_user_dir }}/.ansible/tmp`

## 4.2.0 - 2020-02-13

### Major Changes

  - Migrate molecule driver to Libvirt
  - Migrate molecule verifier to Ansible
  - Support Ubuntu 19.10
  - Bugfix `coredns` with `_kubelet_resolv_conf`
  - Bugfix `podSubnet` with `--extra-config=kubeadm.pod-network-cidr`
  - Disable all addons with `minikube start --install-addons=false`
  - Disable addon `default-storageclass` manually
  - Disable addon `storage-provisioner` manually

## 4.1.0 - 2020-01-16

### Major Changes

  - Default `interpreter_python` with `python3`
  - Bugfix `python3-xml` not exists for openSUSE Leap 15.1

## 4.0.0 - 2019-11-05

### Major Changes

  - Upgrade minimal Ansible support to 2.9.0
  - Upgrade Travis CI test as Ubuntu Bionic based
  - Cleanup supported archives

## 3.5.0 - 2019-10-06

### Major Changes

  - Support openSUSE Leap 15.1
  - Default with Python 3
  - Revamp molecule test with vagrant

## 3.4.0 - 2019-09-18

### Major Changes

  - Run molecule test manually on Travis CI

## 3.3.0 - 2019-08-27

### Major Changes

  - Update for RHEL 7
  - Add Vagrant test for RHEL 7
  - Download archives to `/var/cache/ansible`
  - Upgrade packages if archives not found from `/var/cache/ansible`
  - Debug `--apiserver-port` conflict with dashboard

## 3.2.0 - 2019-07-08

### Major Changes

  - Update LXD test profile for Kubernetes v1.15.0 support
  - Fix molecule `group_vars` with links
  - Replace `with_items` with `loop`
  - Replace `with_dict` with `var`
  - Replace `with_first_found` with `lookup('first_found')`

## 3.1.0 - 2019-06-13

### Major Changes

  - Always include default variables from `vars/main.yml`
  - Always use `become: true` with molecule, especially for vagrant
  - Abstract archive download checksum with multiple version support
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
