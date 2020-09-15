# Crust node
Official crust node service for running crust protocol.

## Preparation work
- Hardware requirements: 

  CPU must contain **SGX module**, and make sure the SGX function is turned on in the bios, please click [this page](https://github.com/crustio/crust/wiki/Check-TEE-supportive) to check if your machine supports SGX

- Operating system requirements:

  Ubuntu 16.04/18.04
  
- Other configurations

  - **Secure Boot** in BIOS needs to be turned off
  - Need use ordinary account, **cannot support root account**

## Install dependencies

### Install crust service
```shell
sudo ./install.sh
```

### Generate application configuration

#### Modify config.yaml
```shell
sudo vim /opt/crust/crust-node/config.yaml
```

### Run crust service and karst service

```shell
sudo systemctl start crust
sudo systemctl start karst
```

## License

[GPL v3](LICENSE)
