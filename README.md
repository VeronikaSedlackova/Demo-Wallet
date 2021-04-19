# Credential Handler API Demo Wallet

## Original Project

This project is based on this repository: [Demo Wallet](https://github.com/digitalbazaar/chapi-demo-wallet)


## Background

It represents one part of an example Verifiable Credential flow:

1. [An example university](https://github.com/VeronikaSedlackova/Demo-Issuer) (issuer)
2. Digital Wallet (this project)
3. [An example bookshop](https://github.com/VeronikaSedlackova/Demo-Verifier) (verifier)



## Local development

1. Run `npm install` (Node.js is necessary)
2. Run `npm start`
3. Visit `https://127.0.0.1:8081` or `https://192.168.178.23:8081`

## Test procedure

1. Click on "Login" to start a wallet session. The wallet content will be "none" (in Demo-Wallet)
2. Click on "Verifiable Credential" to receive a credential with the claim to be a student there. Just follow further instructions (in Demo-Issuer)
3. Optional: If you reload the Demo Wallet you will see the credential from the university. You can click on the credential to see the corresponding DID Document
4. Click on "Bestätigen mit einem Verifiable Credential" to share you Student Credential with the bookshop. Just follow further instructions and click "share" at the end. If you scroll to the bottom you will see the verifiable presentation of the verifiable credential (in Demo-Verifier)

This project can issue only one Verifiable Credential for the user "Alice Doe". If you want to repeat the whole process, just delete the bookshop cookie and reload all pages. 


## License

[New BSD License (3-clause)](LICENSE) © 2020 Digital Bazaar
