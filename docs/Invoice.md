

# Invoice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attachments** | [**OasAnyTypeNotMapped**](.md) |  |  [optional]
**billingPeriodEnd** | [**Date**](Date.md) |  |  [optional]
**billingPeriodStart** | [**Date**](Date.md) |  |  [optional]
**cancellationDate** | [**Date**](Date.md) |  |  [optional]
**cancellationInvoiceId** | **String** | References the invoice entity. |  [optional]
**cancellationReason** | **String** |  |  [optional]
**contractId** | [**UUID**](UUID.md) | References the contract entity. |  [optional]
**currency** | [**CurrencyCode**](CurrencyCode.md) |  | 
**customerId** | **String** | References the customer entity. |  [optional]
**discountAmount** | **String** |  |  [optional]
**discountDays** | **Integer** |  |  [optional]
**discountPercentage** | **String** |  |  [optional]
**documentType** | [**DocumentType**](DocumentType.md) |  |  [optional]
**dunningLevel** | **Integer** |  |  [optional]
**inputVatAmount** | **String** |  |  [optional]
**inputVatDeductible** | **Boolean** |  |  [optional]
**inputVatPercentage** | **String** |  |  [optional]
**introductionText** | **String** |  |  [optional]
**invoiceType** | [**InvoiceType**](InvoiceType.md) |  | 
**isCancelled** | **Boolean** |  |  [optional]
**isDraft** | **Boolean** |  |  [optional]
**isEuAcquisition** | **Boolean** |  |  [optional]
**isEuDelivery** | **Boolean** |  |  [optional]
**isIntraCommunityAcquisition** | **Boolean** |  |  [optional]
**isReverseCharge** | **Boolean** |  |  [optional]
**issueDate** | [**Date**](Date.md) |  | 
**ledgerAccount** | **String** |  |  [optional]
**lineItems** | [**OasAnyTypeNotMapped**](.md) |  | 
**margin25a** | **Boolean** |  |  [optional]
**margin25aGross** | **String** |  |  [optional]
**margin25aPurchasePrice** | **String** |  |  [optional]
**notes** | **String** |  |  [optional]
**orderNumber** | **String** |  |  [optional]
**originalPdfPath** | **String** |  |  [optional]
**paidAmount** | **String** |  |  [optional]
**paymentDueDate** | [**Date**](Date.md) |  |  [optional]
**paymentStatus** | [**PaymentStatus**](PaymentStatus.md) |  |  [optional]
**paymentTermsText** | **String** |  |  [optional]
**precedingSalesVoucherId** | **String** | References the preceding sales voucher entity. |  [optional]
**precedingSalesVoucherType** | [**PrecedingSalesVoucherType**](PrecedingSalesVoucherType.md) |  |  [optional]
**receiptConfirmationAvailable** | **Boolean** |  |  [optional]
**relatedInvoiceId** | [**UUID**](UUID.md) | References the invoice entity. |  [optional]
**relationshipType** | **String** |  |  [optional]
**senderSnapshot** | [**OasAnyTypeNotMapped**](.md) |  |  [optional]
**sentAt** | [**Date**](Date.md) |  |  [optional]
**servicePeriodEnd** | [**Date**](Date.md) |  |  [optional]
**servicePeriodStart** | [**Date**](Date.md) |  |  [optional]
**status** | [**InvoiceStatus**](InvoiceStatus.md) |  | 
**subtotal** | **String** |  | 
**supplierId** | **String** | References the supplier entity. |  [optional]
**taxExemptionReason** | **String** |  |  [optional]
**totalAmount** | **String** |  | 
**totalTax** | **String** |  | 
**vatCountry** | [**CountryCode**](CountryCode.md) |  |  [optional]
**vatSpecialCase** | **String** |  |  [optional]




