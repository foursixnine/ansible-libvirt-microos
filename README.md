# MicroOS on libvirt ansible playbook

Since I needed to create a machine where I'd like to run a k3s sinlgle node cluster, here's how I'd do it so that
I can bring my skills and knowledge to 2023 :D.

## How to use it

`ansible-playbook -i inventory  kvm_example-k3s-vm01.yml`

For the most part, you can take a look at `kvm_example-k3s-vm01.yml`, The configuration of the image is done via
[Combustion](https://en.opensuse.org/Portal:MicroOS/Combustion) see `hosts/roles/kvm/templates/combustion-script.sh.j2`
for more details on how this is implemented, and where I took the script from.

I used https://www.redhat.com/sysadmin/build-VM-fast-ansible to get started and modified contents over time.
