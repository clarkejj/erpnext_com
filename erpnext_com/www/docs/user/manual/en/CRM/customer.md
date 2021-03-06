<!-- add-breadcrumbs -->
# Customer

A customer, who is sometimes known as a client, buyer, or purchaser is the one
who receives goods, services, products, or ideas, from a seller for a monetary
consideration. A customer can also receive goods or services from a vendor or
a supplier for other valuable considerations.

A customer is uniquely identified by the Customer ID. Normally this ID is identical to the customer Full Name, but in case of duplicate Full Name, a Name-1 is created as ID.

### 1. How to create a Customer

1. You can crete Customers via **CRM > Sales Pipeline > New** or **Selling > Customers > New**.
1. Enter Customer name.
1. Set the Customer group whether Commercial, Individual etc.
1. You can set From Lead if you go this customer from a lead.
1. Ticking Disabled will hide the customer from the Customer List.
1. The Is Internal Customer checkbox is for a person from one of your companies who is a customer to another one of your companies. See more [here](/docs/user/manual/en/accounts/inter-company-invoices).
1. Save.

    <img class="screenshot" alt="Create Customer" src="{{docs_base_url}}/assets/img/crm/create-customer.gif">

1. You can also upload customer details via the [Data Import Tool](/docs/user/manual/en/setting-up/data/data-import).

### 2. Features
A Customer can avail the features (operations) in the selling process. The general flow can be summarized as:

<img class="screenshot" alt="Customer" src="{{docs_base_url}}/assets/img/crm/customer-to selling-flowchart.jpeg">

> Note: Customers are separate from Contacts and Addresses. A Customer can
have multiple Contacts and Addresses.

#### 2.1 Contacts and Addresses

[Contacts and Addresses](/docs/user/manual/en/CRM/contact) in ERPNext are stored separately so that you can
attach multiple Contacts or Addresses to Customers and Suppliers

Thus we may have identical Customer Names that are uniquely identified by the ID. Since the email address is not part of the
customer information, the linking of Customer and User is through Contacts.

#### 2.2 Integration with Accounts

In ERPNext, there is a separate Account record for each Customer, for each
Company.

When you create a new Customer, ERPNext will automatically create an Account
Ledger for the Customer under “Accounts Receivable” in the Company set in the
Customer record.

> Advanced Tip: If you want to change the Account Group under which the
Customer Account is created, you can set it in the Company master. If you want
to create an Account in another Company, just change the Company value and
“Save” the Customer again.

By default, the system does not generate an account for every customer. All
Customers can be booked in one account called Debitors. In order to manage a
separate account for each customer, you have to first create the account under
Accounts Receivable in the [Chart of Accounts](/docs/user/manual/en/accounts/chart-of-accounts.html) and then add it on the customer's
form accounts table.

#### 2.3 Customer Settings

You can link a Price List to a Customer (select “Default Price List”), so that
when you select that Customer, the Price List will be automatically selected.

You can set “Credit Days”, so that it is automatically set due date in the Sales
Invoices made against this Customer. Credit Days can be defined as fixed days or last day of the next month based on invoice date.

You can set how much credit you want to allow for a Customer by adding the
“Credit Limit”. You can also set a global “Credit Limit” in the Company
master. Classifying Customers

ERPNext allows you to group your Customers using [Customer Group](/docs/user/manual/en/CRM/setup/customer-group.html)
and also divide them into [Territories](/docs/user/manual/en/setting-up/territory.html)
Grouping will help you get better analysis of your data and
identify which Customers are profitable and which are not. Territories will
help you set sales targets for the respective territories.
You can also mention [Sales Person](/docs/user/manual/en/CRM/setup/sales-person.html) against a customer.


<div>
    <style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
    </style>
    <div class='embed-container'>
        <iframe src='https://www.youtube.com/embed//zsrrVDk6VBs?end=212' frameborder='0' allowfullscreen>
        </iframe>
    </div>
</div>

#### 2.6 Sales Partner

A Sales Partner is a third party distributor / dealer / commission agent /
affiliate / reseller who sells the companies products, for a commission. This
is useful if you make the end sale to the Customer, involving your Sales
Partner.

If you sell to your Sales Partner who in-turn sells it to the Customer, then
you must make a Customer instead.

#### 3. Related Topics
1. [Customer Group](/docs/user/manual/en/CRM/setup/customer-group)
1. [Quotation](/docs/user/manual/en/selling/quotation)