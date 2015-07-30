CA-bundles
==============

# About

A repository of CA bundles for testing purposes

## DOD CAs
* Contains all recent DOD CAs up to CA-30 and DOD CA Email up to CA-30


## Public CAs
* Up to date as of 20150626 

* There are now 905 intermediate CAs in the package (up from 765)
* The bundle package now optionally includes the Microsoft Trusted Root package certificates (there are 341 Trusted Roots in the typical Microsoft trust store, as opposed to 180 in the newest Mozilla store)
* The certificate base used to collect these trust details was collected from 125,000 random site selections, ALL SSL-enabled hosts in the Alexa Top 1 Million, and any identified AIA sources from trusted providers. It represents as complete a picture of SSL trust on the Internet as can be derived

* intermediate-ca-bundle.crt
* intermediate-ca-bundle-light.crt
   Just the Intermediate CAs whose trust path can be chained up to the recognized trusted roots. The "light" version of the file removes the human-readable text, leaving just the PEM certificates.
 
* blended-bundle.crt
* blended-bundle-light.crt
   A bundle of both trusted roots and intermediates drawn from both Microsoft and NSS roots. The "light" version of the file removes the human-readable text, leaving just the PEM certificates. This bundle is perhaps the best one to use
 
* root-ca-bundle-msft.crt
* root-ca-bundle-mozilla.crt
* root-ca-bundle-integrated.crt
   The Root CA trust list broken out by provider (Microsoft/NSS), or bundled unique certificates. This JUST consists of the Root CAs - no intermediates

# Disclaimer
 These are provided for testing purposes only, you should verify the validity of these certificates individually. These are to be used for testing purposes only

 I did not assemble these bundles