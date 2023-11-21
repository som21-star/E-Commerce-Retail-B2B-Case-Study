# E-Commerce-Retail-B2B-Case-Study
It's a binary classification problem statement with class-imbalance issue. We dealt with SMOTE+TOMEK and ADASYN
Result
Accuracy:  0.9778936910084451
F1 score:  0.9883692709791841
Recall:  0.9771502399409376
Precision:  0.9998489140698772
Helped clients to find the business recommendations and generate insights through the analysis.

Problem Statement

Schuster is a multinational retail company dealing in sports goods and accessories. Schuster conducts significant business with hundreds of its vendors, with whom it has credit arrangements. Unfortunately, not all vendors respect credit terms and some of them tend to make payments late. Schuster levies heavy late payment fees, although this procedure is not beneficial to either party in a long-term business relationship. The company has some employees who keep chasing vendors to get the payment on time; this procedure nevertheless also results in non-value-added activities, loss of time and financial impact. Schuster would thus try to understand its customers’ payment behaviour and predict the likelihood of late payments against open invoices.

Goal

Schuster would like to better understand the customers’ payment behaviour based on their past payment patterns (customer segmentation). Using historical information, it wants to be able to predict the likelihood of delayed payment against open invoices from its customers. It wants to use this information so that collectors can prioritise their work in following up with customers beforehand to get the payments on time.

Data Understanding

RECEIPT_METHOD In which method payments have been made

CUSTOMER_NAME Name of the customer/vendor

CUSTOMER_NUMBER Customer's unique identity number

RECEIPT_DOC_NO Reference number of the payment receipt

RECEIPT_DATE The date in which the payment has been made

CLASS As the payment against these invoices have already been received so Transaction Class as PMT (short for Payment) assigned

CURRENCY_CODE Currency used for the payment

Local Amount Invoice value in local currency

USD Amount Invoice Value converted to USD

INVOICE_ALLOCATED Invoice number that has been allocated to a particular vendor

INVOICE_CREATION_DATE The date on which the invoice was created

DUE_DATE The date by which the payment was to be made

PAYMENT_TERM Days given to the vendor/customer for making the payments

INVOICE_CLASS Three types of Invoice classes - Credit Memo or Credit Note (CM), Debit Memo or Debit Note (DM) or Invoice (INV)

INVOICE_CURRENCY_CODE Currency code as per the invoice generated

INVOICE_TYPE Invoice created for physical goods or services (non-goods)

Finally target variable will be derived based on the suggested information "You need to derive it by checking whether the payment receipt date falls within, or after the due date. By doing so, you can create your binary target variable as 1 or 0."

Top 10 factors / important predictors

age payment_term_50% advance payment and 50% upon receiving the shipment payment_term_eom payment_term_lcsight payment_term_on consignment invoice_currency_code_eur invoice_currency_code_gbp invoice_currency_code_kwd invoice_currency_code_qar invoice_type_non goods

Recommendations

We should focus more on the time difference between Due Date and Invoice Payment Date
Payment terms: 50% advance payment and 50% upon receiving the shipment, eom, lcsight and on consignment variables need to be considered with greater attention.
Where the invoice currency codes are eur, gbp, kwd and qar, the risk is higher of delay payment.
Invoice type non-goods has lower impact than Goods invoice type in delayed payment.
