# thingy.jp certs

This repo contains:
* The root cert - needs to be installed on devices
* The current intermediate cert - will be part of any supplied cert bundles
* The current server signing cert - will be part of supplied server cert bundles
* The current device signing cert - will be part of supplied device cert bundles

Expiry rules:
* The root is valid for 50 years from 2018/06/23.
* Any intermediates and device signing certs will expire at the same time as the
root but may become valid at a later date.
* Any server signing certs will have a validity of 5 years from the creation
time.
* Issued device certs will have no expiry.
* Issued server certs will have a validity of 1 year from the creation time.

root and intermediate security:
* root and intermediate private key creation and certificate signing were done with a Nitrokey HSM (https://shop.nitrokey.com/shop/product/nitrokey-hsm-7) 
