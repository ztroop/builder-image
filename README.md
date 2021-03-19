# Builder Image

A docker image with `docker`, `vagrant`, `packer`, `libvirt`, `kvm` and other development tools installed to make continuous integration builds as easy as possible!

### Goals

- Supporting **docker-in-docker (DIND)** and **vm-in-docker (VIND)** operation out of the box.
- Provide an up-to-date, easy and flexible image to work with out of the box.

### Technical Notes

If you're looking at **vm-in-docker (VIND)** operation, online search results will suggest you run the container with `--privileged` to access the `kvm` device. **DO NOT** need to do this. You can specify `--device=/dev/kvm` instead.