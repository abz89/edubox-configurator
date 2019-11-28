# EDUBOX CONFIGURATOR

Setup/manage "Edubox Router" device with Ansible but without Python.

## Requirements

\*Ansible (Of course :D)

Debian/Ubuntu

```
sudo apt install ansible
```

MacOS with Homebrew

```
brew install ansible
```

\*Ansible Role: openwrt as dependencies

```
ansible-galaxy install gekmihesg.openwrt
```

## Usage

- copy `vars.yml.example` to `vars.yml` then edit accordingly.
- edit host in `invetory` file as needed.
- create and edit `authorized_keys` with desired ssh key.
- place the desired openwrt firmware image to `image.bin`.
- run `ansible-playbook setup.yml` for flashing custom firmware then config, or
- run `ansible-playbook config.yml` for running config, or

## License

GNU General Public License v3.0 (see https://www.gnu.org/licenses/gpl-3.0.txt)
