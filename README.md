# swiftfref-sdk-java

## Requirements

Building the API client library requires [Maven](https://maven.apache.org/) to be installed.

## Installation

To install the API client library to your local Maven repository, simply execute:

```bash
mvn install
```

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
    <groupId>com.swift.swiftref</groupId>
    <artifactId>swiftref-sdk-java</artifactId>
    <version>0.0.0</version>
    <scope>compile</scope>
</dependency>
```

### Others

At first generate the JAR by executing:

    mvn package

Then manually install the following JARs:

* target/swiftref-sdk-java-0.1.0.SNAPSHOT.jar
## Example of API Endpoints

All URIs are relative to *https://api.swiftrefdata.com/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BbansApi* | [**getIbanFromBban**](docs/BbansApi.md#getIbanFromBban) | **GET** /bbans/{bban}/iban | Get the IBAN from a BBAN
*BicsApi* | [**getBicDetails**](docs/BicsApi.md#getBicDetails) | **GET** /bics/{bic} | Get details of a BIC
*BicsApi* | [**getBicValidity**](docs/BicsApi.md#getBicValidity) | **GET** /bics/{bic}/validity | Check validity of a BIC
*BicsApi* | [**getLeiFromBic**](docs/BicsApi.md#getLeiFromBic) | **GET** /bics/{bic}/lei | Get the LEI for a BIC
*BicsApi* | [**getNationalIdsFromBic**](docs/BicsApi.md#getNationalIdsFromBic) | **GET** /bics/{bic}/national_ids | Get National IDs for a BIC
*BicsApi* | [**getSepaReachabilityFromBic**](docs/BicsApi.md#getSepaReachabilityFromBic) | **GET** /bics/{bic}/reachability | Validate SEPA reachability of a BIC
*BicsApi* | [**getSsisFromBic**](docs/BicsApi.md#getSsisFromBic) | **GET** /bics/{bic}/ssis | Get SSIs for a BIC
*IbansApi* | [**getBicFromIban**](docs/IbansApi.md#getBicFromIban) | **GET** /ibans/{iban}/bic | Get the BIC for an IBAN
*IbansApi* | [**getIbanDetails**](docs/IbansApi.md#getIbanDetails) | **GET** /ibans/{iban} | Get details for an IBAN
*IbansApi* | [**getIbanValidity**](docs/IbansApi.md#getIbanValidity) | **GET** /ibans/{iban}/validity | Check validity of an IBAN
*LeisApi* | [**getBicFromLei**](docs/LeisApi.md#getBicFromLei) | **GET** /leis/{lei}/bic | Get the BIC for an LEI
*NationalIdsApi* | [**getBicsFromNationalId**](docs/NationalIdsApi.md#getBicsFromNationalId) | **GET** /national_ids/{national_id}/bics | Get BICs of a National ID
*NationalIdsApi* | [**getNationalIdDetails**](docs/NationalIdsApi.md#getNationalIdDetails) | **GET** /national_ids/{national_id} | Get details of a National ID
*NationalIdsApi* | [**getNationalIdValidity**](docs/NationalIdsApi.md#getNationalIdValidity) | **GET** /national_ids/{national_id}/validity | Check the Validity of a National ID


## Documentation for Models

 - [Address](docs/Address.md)
 - [Bic](docs/Bic.md)
 - [BicDetails](docs/BicDetails.md)
 - [BicValidity](docs/BicValidity.md)
 - [Bics](docs/Bics.md)
 - [ContactDetails](docs/ContactDetails.md)
 - [CorrespondentBic](docs/CorrespondentBic.md)
 - [Iban](docs/Iban.md)
 - [IbanBic](docs/IbanBic.md)
 - [IbanDetails](docs/IbanDetails.md)
 - [IbanValidity](docs/IbanValidity.md)
 - [IntermediaryBic](docs/IntermediaryBic.md)
 - [Lei](docs/Lei.md)
 - [NationalId](docs/NationalId.md)
 - [NationalIdDetails](docs/NationalIdDetails.md)
 - [NationalIdValidity](docs/NationalIdValidity.md)
 - [NationalIds](docs/NationalIds.md)
 - [NationalIdsDetails](docs/NationalIdsDetails.md)
 - [SepaPaymentChannel](docs/SepaPaymentChannel.md)
 - [SepaReachability](docs/SepaReachability.md)
 - [Ssi](docs/Ssi.md)
 - [Ssis](docs/Ssis.md)
 - [Status](docs/Status.md)
 - [SwiftService](docs/SwiftService.md)


## Documentation for Authorization

Authentication schemes defined for the API:
### basicAuth

- **Type**: HTTP basic authentication


## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Development
* [Source Control](https://github.com/swiftinc/swiftref-sdk-java)


