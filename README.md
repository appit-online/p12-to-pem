# [p12-to-pem-converter: Node.js](https://github.com/appit-online/p12-to-pem)

Convert PKCS12/.p12-files into pem key and pem certificate.



**Table of contents:**


* [Quickstart](#quickstart)

  * [Installing the library](#installing-the-library)
  * [Using the library](#using-the-library)
* [License](#license)

## Quickstart

### Installing the library

```bash
npm install p12-pem --save
```


### Using the library

```javascript
import * as p12 from 'p12-pem';

/**
 * Given a p12 file, convert it to the PEM format.
 * @param {string} pathToCert The relative path to a p12 file.
 * @param {string} password of p12 / private key.
 */
const {pemKey, pemCertificate, commonName} = p12.getPemFromP12(certPath, password);
console.log('The converted private key in PEM:');
console.log(pemKey);

console.log('The converted certificate in PEM:');
console.log(pemCertificate)

console.log('The extracted commonName:');
console.log(commonName);

```

## Supported Node.js Versions

Our client libraries follow the [Node.js release schedule](https://nodejs.org/en/about/releases/).
Libraries are compatible with all current _active_ and _maintenance_ versions of
Node.js.

## License

Apache Version 2.0

See [LICENSE](https://github.com/appit-online/p12-to-pem/blob/master/LICENSE)
