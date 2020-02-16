# iOS-decryption-keys

#### decryption keys for iOS firmwares (json format). Can be easily read by Python json module.

## Usage:
+ Read iPad3,1 iOS9.1 DeviceTree key and IV <br />
``` Python
import json

list = json.load(open("firmware-keys-iPad3,1.json"))

devicetree_key = list['iPad3,1']['9.1']['keys']['devicetree']
devicetree_iv = list['iPad3,1']['9.1']['ivs']['devicetree']
print("Key: " + devicetree_key)
print(" IV: " + devicetree_iv)
```