# UaiCoin-Blockchain-Explorer
Block explorer for UaiCoin CryptoNote based cryptocurrency.

#### Installation

1) It takes data from daemon UaiCoind. It should be accessible from the Internet. Run UaiCoin with open port as follows:
```bash
./UaiCoind --enable-cors="*" --enable_blockexplorer --rpc-bind-ip=0.0.0.0 --rpc-bind-port=21898
```
2) Just upload to your website and change 'api' variable in config.js to point to your daemon.

#### Installation for Mac on localhost

```bash
sudo su -
apachectl start
./UaiCoind --enable-cors="*" --enable_blockexplorer --rpc-bind-ip=0.0.0.0 --rpc-bind-port=21898
```
In Finder, Go > Go To Folder: /Library/WebServer/Documents
Download and extract this repository to /Library/WebServer/Documents/block-explorer
Go to http://localhost/block-explorer/
If it does not work, open http://127.0.0.1:21898/getinfo and see in your local daemon if it's accepting connections

Additional resource: https://jason.pureconcepts.net/2012/10/install-apache-php-mysql-mac-os-x/

### Development
Devs:
    @devopsralf

Donate: [TRTL] TRTLv2RCPuD7AaaVpQkRPF59MMLx5WW3qFxwJz4Doy7dHhNA6UuQjEpLL3rpUQS4RXdQn8fb4P1XC3K62GeJjGgG8DP9LNaTrNL

### Note

A lot of this code is from the great Karbovanets/Karbowanec-Blockchain-Explorer
