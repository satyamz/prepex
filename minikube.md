# Installing *Minikube* on *Linux*

## Before you begin
VT-x or AMD-v virtualization must be enabled in your computer’s BIOS.

## Install a Hypervisor

If you do not already have a hypervisor installed, install the appropriate one for your OS now:

- macOS: VirtualBox or VMware Fusion, or HyperKit.

- Linux: VirtualBox or KVM.

- Windows: VirtualBox or Hyper-V.

> Note: Minikube also supports a --vm-driver=none option that runs the Kubernetes components on the host and not in a VM. Using this driver requires Docker, but not a hypervisor.

## Linux systems

```shell
curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.29.0/minikube-linux-amd64 && chmod +x minikube && sudo cp minikube /usr/local/bin/ && rm minikube
```

## Mac systems
```
brew cask install minikube
```

## Windows systems
Download the `minikube-windows-amd64.exe` file, rename it to `minikube.exe` and add it to your path.

`https://github.com/kubernetes/minikube/releases/tag/v0.29.0`