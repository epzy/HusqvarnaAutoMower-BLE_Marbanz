# AutoMower-BLE

This is an unofficial reverse-engineered Husqvarna Automower Connect BLE library. It allows connecting and controlling an Automower without any accounts, cloud, or network connection.

This library was originally developed by Alistair23, but it is now maintained and further developed by Marbanz. The current development is focused on integrating and testing with a **Gardena Sileno Minimo 250**, though it should still work with other Automower models. If you are able to test on different models, please do and report any results back.

Details on the original reverse engineering process are available at: https://www.alistair23.me/2024/01/06/reverse-engineering-automower-ble

## Installation
You can install this library directly from the repository:

```shell
pip3 install git+https://github.com/Marbanz/AutoMower-BLE.git
```

Please note that the library is under active development and may not yet be released on pip.

## Testing Connections

You can test querying data with the following:

```shell
python -m automower_ble.mower --address D8:B6:73:40:07:37
```

```shell
python -m automower_ble.mower --address D8:B6:73:40:07:37 --command park
```

Where command is one of:
  park  
  pause  
  override  
  resume  

(override will run for 3hrs)
