# iOS-decryption-keys

#### decryption keys for iOS firmwares (json format). Can be easily read by Python json module.

## Usage:
+ Read iPad3,1 iOS9.1 DeviceTree key and IV <br />
``` Python
import json

keylist = json.load(open("firmware-keys-iPad3,1.json"))

devicetree_key = keylist['iPad3,1']['9.1']['keys']['devicetree']
devicetree_iv = keylist['iPad3,1']['9.1']['ivs']['devicetree']
print("Key: " + devicetree_key)
print(" IV: " + devicetree_iv)
```