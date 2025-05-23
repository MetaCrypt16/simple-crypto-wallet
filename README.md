# simple-crypto-wallet
A minimal Crypto wallet that performs the basic operations like generating key pair ,Ethereum address , Sign and Verify the signature and also fetch the balance using public key api
#Features

-->Generate Key pair used ecdsa(elliptic curve Digital Signature Algorithm) library to import the Signing key and SECP256k1(Which is the standards for efficient cryptography) so as to generate the private key and the corresponding public key

-->Generating the Ethereum Address Since the public key is very large so it is important to shorten it ,mainly for two main reasons 1.Compactness 2.Security

In Ethereum there is a set patter for generating the address for this we import eth-hash[pycryptodome] so as to import keccak_256

keccak_256 is the hashing algorithm in Ethereum which hashes the public key and then we take the last 20 characters of the hashed key and prepend 0x for a valid address

#Screenshots are shown in GitHub

-->Sign and verify A important feature of the wallet is to sign and to ensure the message is being signed by the correct person Signature is done by the private key and It is verified by it's corresponding public key to ensure it has been signed by the correct person

#Screenshots attached in the folder

-->Fetching the balance via Public api For api blockLauncher is being used

#Refer to screenshots

