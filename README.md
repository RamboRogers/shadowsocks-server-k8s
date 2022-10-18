# ShadowSocks K8s Server

I wrote this example for my lab because the example using helm on the official site is complicated and didn't work for me.  This uses the [shadowsocks-rust](https://github.com/shadowsocks/shadowsocks-rust) prebuilt containers.

## Installation

Copy the yaml file, edit the password and apply.  The existing lable for locallb is from the my usage of MetalLB.  You need to configure you own service exposure, the port name is ss-443.

```
wget https://raw.githubusercontent.com/RamboRogers/shadowsocks-server-k8s/master/shadowsocks-server.yaml
kubectl apply -f shadowsocks-server.yaml
```

## Usage


* Add to your shadowsocks client with the password.  
* This server also works without Outline VPN.


## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)