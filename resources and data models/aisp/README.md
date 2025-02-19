---
layout: default
title: AISP
nav_order: 1
---

# AISP Resources and Data Models - v3.1.2

Resources accessed using the aisp PSD2 role are detailed here:

* [Account Access Consents](Account%20Access%20Consents.md)
* [Accounts](Accounts.md)
* [Balances](Balances.md)
* [Transactions](Transactions.md)
* [Beneficiaries](Beneficiaries.md)
* [Direct Debits](Direct%20Debits.md)
* [Standing Orders](Standing%20Orders.md)
* [Products](Products.md)
	* [BCA Product Data Model](BCA%20Product%20Data%20Model.md)
	* [PCA Product Data Model](PCA%20Product%20Data%20Model.md)
	* [Other Product Data Model](Other%20Product%20Data%20Model.md)
* [Offers](Offers.md)
* [Parties](Parties.md)
* [Scheduled Payments](Scheduled%20Payments.md)
* [Statements](Statements.md)


## Endpoints

The API endpoints for these resources, and their mandatory/conditional/optional status are given below.

| Resource |Endpoints |Mandatory? |
| --- |--- |---|
| [account-access-consents](Account%20Access%20Consents.md) |POST /account-access-consents |Mandatory |
| [account-access-consents](Account%20Access%20Consents.md) |GET /account-access-consents/{ConsentId} |Mandatory |
| [account-access-consents](Account%20Access%20Consents.md) |DELETE /account-access-consents/{ConsentId} |Mandatory |
| [accounts](Accounts.md) |GET /accounts |Mandatory |
| [accounts](Accounts.md) |GET /accounts/{AccountId} |Mandatory |
| [balances](Balances.md) |GET /accounts/{AccountId}/balances |Mandatory |
| [balances](Balances.md) |GET /balances |Optional |
| [transactions](Transactions.md) |GET /accounts/{AccountId}/transactions |Mandatory |
| [transactions](Transactions.md) |GET /transactions |Optional |
| [beneficiaries](Beneficiaries.md) |GET /accounts/{AccountId}/beneficiaries |Conditional |
| [beneficiaries](Beneficiaries.md) |GET /beneficiaries |Optional |
| [direct-debits](Direct%20Debits.md) |GET /accounts/{AccountId}/direct-debits |Conditional |
| [direct-debits](Direct%20Debits.md) |GET /direct-debits |Optional |
| [standing-orders](Standing%20Orders.md) |GET /accounts/{AccountId}/standing-orders |Conditional |
| [standing-orders](Standing%20Orders.md) |GET /standing-orders |Optional |
| [products](Products.md) |GET /accounts/{AccountId}/products |Conditional |
| [products](Products.md) |GET /products |Optional |
| [offers](Offers.md) |GET /accounts/{AccountId}/offers |Conditional |
| [offers](Offers.md) |GET /offers |Optional |
| [parties](Parties.md) |GET /accounts/{AccountId}/parties |Conditional |
| [parties](Parties.md) |GET /accounts/{AccountId}/party |Conditional |
| [parties](Parties.md) |GET /party |Conditional |
| [scheduled-payments](Scheduled%20Payments.md) |GET /accounts/{AccountId}/scheduled-payments |Conditional |
| [scheduled-payments](Scheduled%20Payments.md) |GET /scheduled-payments |Optional |
| [statements](Statements.md) |GET /accounts/{AccountId}/statements |Conditional |
| [statements](Statements.md) |GET /accounts/{AccountId}/statements/{StatementId} |Conditional |
| [statements](Statements.md) |GET /accounts/{AccountId}/statements/{StatementId}/file |Optional |
| [statements](Statements.md) |GET /accounts/{AccountId}/statements/{StatementId}/transactions |Conditional |
| [statements](Statements.md) |GET /statements |Optional |

### Notes

Definitions for Mandatory, Conditional and Optional are given in the [Read/Write Data API Profile](../../profiles/read-write-data-api-profile.md#categorisation-of-implementation-requirements).

## Account and Transactionns Resource Compatibility

|  | |Read-Write API Profile |Read-Write API Profile |Read-Write API Profile |Account and Transaction API Profile |Account and Transaction API Profile |Account and Transaction API Profile |
| --- |--- |--- |--- |--- |--- |--- |--- |
|  | |v3.1 |v3.1.1 |3.1.2 |v3.1 |v3.1.1 |3.1.2 |
| Account Access Consents |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Accounts |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Balances |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Beneficiaries |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Direct Debits |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Offers |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Parties |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Products |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Scheduled Payments |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Standing Orders |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Statements |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
| Transactions |v3.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.1 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
|  |v3.1.2 |TRUE |TRUE |TRUE |TRUE |TRUE |TRUE |
