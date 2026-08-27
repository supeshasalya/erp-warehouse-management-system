# Inventory & Warehouse Management System

A web-based inventory and warehouse management system developed as a freelance software project for managing products, suppliers, stock movements, warehouse documents, and expired inventory through a centralized system.

## Overview

The system supports day-to-day warehouse operations while maintaining accurate stock records at product, pack, box, and individual-item levels.

It provides dedicated workflows for receiving stock, issuing stock, monitoring current inventory, maintaining product-level Bin Cards, handling expired goods, supplier returns, stock adjustments, and generating printable operational documents.

## Key Features

### Product Management
- Add and manage products
- Maintain product codes, names, and pack sizes
- Track inventory using boxes and individual items
- Support different pack sizes for different products

### Supplier Management
- Add and manage suppliers
- Associate products and stock transactions with suppliers
- Filter inventory information by supplier

### Goods Received Notes (GRN)
- Create GRNs for incoming stock
- Select the relevant supplier and lorry
- Add multiple products to a GRN
- Record pack size, boxes, and individual items received
- Update inventory through receiving transactions
- Generate print-ready GRNs
- Maintain GRN records for future reference

### Loading Issue Notes
- Create issue notes when stock is issued from the warehouse
- Select products and specify boxes/items to issue
- Validate requested quantities against available stock
- Prevent issuing quantities greater than available inventory
- Record supplier, lorry, cash collector, and authenticator details
- Generate printable issue notes
- Maintain issue-note records

### Unloading Issue Notes
- Record stock movements associated with unloading operations
- Track quantities using the box/item stock structure
- Maintain movement history for stock calculations

### Current Stock
- View current inventory across products
- Filter by supplier and product
- Search by product code, name, or pack size
- Display stock as full boxes, remaining items, and total pieces
- Provide a consolidated warehouse stock view

### Bin Card / Stock Card
- View product-level stock movement history
- Select a product and date range
- Display opening balance
- Track IN and OUT movements
- Calculate the running balance after each transaction
- Display balances using boxes and individual items
- Generate a printable Bin Card / Stock Card

### Expired Store
- Maintain a separate store for expired inventory
- Record expired products returned from retail shops
- Keep expired stock separate from main inventory
- View expired quantities by product and supplier
- Search and filter expired inventory
- Return expired goods to suppliers
- Track expired-store movements

### Stock Adjustment
- Correct system stock when physical stock does not match recorded stock
- Support controlled inventory reconciliation

### Printing & Documentation
The system provides print-ready documents for operational use, including:
- Goods Received Notes (GRNs)
- Loading Issue Notes
- Unloading Issue Notes
- Bin Cards / Stock Cards
- Expired-stock movement records

## Inventory Tracking

Stock is maintained using:

`Boxes + Individual Items = Total Pieces`

For example:

`1 box + 12 items = 32 pieces`

The configured pack size is used consistently when calculating and displaying inventory across receiving, issuing, current-stock reports, and Bin Cards.

## Stock Validation

Issue transactions are validated against the available stock.

For example, if a product has:

`1 box + 12 items`

the system prevents a user from entering a quantity such as:

`5 boxes`

and displays a validation message indicating that the requested quantity exceeds the available stock.

This helps prevent accidental over-issuing and improves inventory accuracy.

## Dashboard

The dashboard provides a centralized overview of the system, including:
- Total products
- Out-of-stock products
- Low-stock products
- Multi-pack products
- Quick access to Bin Cards / Stock Cards
- Expired Notes
- Expired Store
- Stock Adjustments
- Issue Lorry management

## Main Workflows

### Receiving Stock

```text
Supplier
   ↓
Create GRN
   ↓
Select Lorry
   ↓
Add Products
   ↓
Enter Boxes / Items
   ↓
Submit GRN
   ↓
Inventory Updated
```

### Issuing Stock

```text
Current Stock
   ↓
Create Issue Note
   ↓
Select Products
   ↓
Enter Boxes / Items
   ↓
Validate Available Stock
   ↓
Submit Issue Note
   ↓
Inventory Updated
```

### Stock Monitoring

```text
Stock Transactions
       ↓
  Current Stock
       ↓
   Bin Card
       ↓
IN / OUT History
       ↓
Running Balance
```

### Expired Stock

```text
Expired Goods
     ↓
Expired Note
     ↓
Expired Store
     ↓
Track Expired Stock
     ↓
Return to Supplier
```

## Core Modules

| Module | Purpose |
|---|---|
| Dashboard | Inventory overview and quick access |
| Products | Product and pack-size management |
| Suppliers | Supplier management |
| GRN | Record incoming stock |
| Loading Issue Note | Record stock issued from the warehouse |
| Unloading Issue Note | Record unloading-related movements |
| Current Stock | View and filter current inventory |
| Bin Card | Product-level stock movement history |
| Expired Note | Record expired goods |
| Expired Store | Manage separated expired inventory |
| Stock Adjustment | Reconcile physical/system stock |
| Issue Lorry | Manage lorries used for issue operations |
| Printing | Generate operational documents |

## Highlights

- End-to-end warehouse inventory workflow
- Transaction-based stock tracking
- Box and individual-item calculations
- Real-time quantity validation during issuing
- Product-level running balances
- Separate expired-stock management
- Supplier return workflow
- Search and filtering across inventory data
- Print-ready business documentation
- Centralized operational dashboard

## Technology

> Replace the placeholders below with the actual technologies used.

```text
Frontend: [Technology]
Backend:  [Technology]
Database: [Technology]
Other:    [Libraries / Tools]
```

## Screenshots

### Dashboard
![Dashboard](screenshots/dashboard.png)

### Current Stock
![Current Stock](screenshots/current-stock.png)

### Bin Card / Stock Card
![Bin Card](screenshots/bin-card.png)

### Expired Store
![Expired Store](screenshots/expired-store.png)

### Loading Issue Note
![Loading Issue Note](screenshots/loading-issue-note.png)

### GRN
![GRN](screenshots/grn.png)

### Product Selection & Stock Validation
![Stock Validation](screenshots/stock-validation.png)

### Login
![Login](screenshots/login.png)

## Installation

> Replace these commands with the actual setup instructions for the project.

```bash
git clone <repository-url>
cd <project-directory>

<install-command>

<start-command>
```

## Project Status

Completed freelance software project.

## Author

Developed as a freelance software project.

---

The system was designed around practical warehouse workflows, with emphasis on accurate stock movement, operational validation, product-level traceability, expired-stock handling, and standardized printable documentation.
