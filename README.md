# rust-os-dev

The image is available on [Docker Hub](https://hub.docker.com/r/swegmann/rust-os-dev/)

Docker environment to build a development environment for building Rust based Operating Systems.

The setup is based on the explanations in the [IntermezzOS](https://intermezzos.github.io/) tutorial and comes with

* SSL certificates
* build-essentials
* `nasm`
* Rust 2016-05-26 via Rustup
* GRUB tools to build images
* `xorriso`

The path `/source` is a volume where you can mount source code from the host machine.

## Usage

The following command will drop you into a Bash shell with the current directory on the host shared.

``` bash
docker run -it --rm -v $(pwd):/source swegmann/rust-os-dev
```

## License

[MIT](http://opensource.org/licenses/MIT)
