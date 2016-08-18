# Garage Sale Helper

## General
A web application which is able to manage different garage sales with similar functionality to Amazon and Ebay. It utilizes the Play framework for Java, the Model-View-Controller paradigm, and Agile development principles.

This application will allow its users to plan, organize, implement, and close out a yard sale.

## User Roles:
A user has a role in each garage sale in which they participate. This role is assigned by creating a sale or by the sale administrator. Note that users may have a different role for each sale in which they participate.

**SuperUser**: The role of SuperUser is a global role that allows the user all privileges, including disabling and unlocking users and acting as the Sale Administrator for any sale.

**Sale Administrator**: The user who opens (or creates) a sale is automatically assigned the role of Sale Administrator (SA) for this sale. The SA may assign the Sale Administrator role to any other user which gives them the same authority over the sale as the original SA. The SA has authority to access all of the features available within a sale, including closing it. The SA also has the authority to assign any of the other roles to any user for this sale.

**Seller**: A seller has access to update the catalog, change prices, initiate advertising, print tags, etc. In other words, a seller can do anything the clerk, cashier, and bookkeeper can do.

**Clerk**: A clerk has access to view the catalog, print tags, view catalog reports, etc.

**Cashier**: A cashier has access to sell items and create receipts.

**Bookkeeper**: A bookkeeper has access to the financial reporting features.

**Guest**: A guest is allowed to browse the catalog and bid on items when that feature is available. By default, all users are granted Guest access into all sales.

## Features
* Login/Registration
* Viewing profiles
* Creating a sale
* Adding/updating items
* Printing tags
* Viewing financial reports
* Closing a sale
* Super User privileges
  * Unlocking/locking accounts
  * Viewing user list
  
## Extra Features
* Using Facebook to advertise a sale
* MySQL database with jdbc connectivity and ebean mapping
* Users can concurrently use the database
* Prices can be changed to support hagglers and bidding
* Additional financial reports
* Photos can be stored for catalog descriptions
* Email receipts provided
