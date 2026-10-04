# Final App Specification — PERFECT PRINTING HOUSE

## Product
Android mobile Sales / Delivery Challan Book. Offline-first. No GST/tax.

## Screens
1. Home — New Challan, History, Settings.
2. New/Edit Challan — automatic number, date, customer, mobile, address, item rows, total, remarks, save/delete.
3. History — search by customer or challan number; open/edit; PDF/share; print.
4. Settings — company name, phone and address.

## Business Rules
- New number = maximum saved challan number + 1.
- Editing keeps the original challan number and date.
- Total = sum(quantity × rate).
- Blank item rows are not written to the database.
- Customer name and at least one named item are required.
- No GST, CGST, SGST, IGST, tax or tax calculations exist.

## Storage
SQLite database stored locally on the Android device. No cloud, login or internet dependency for daily use.

## PDF / Printing
A4 PDF with company heading, challan number/date, customer details, item table, total, remarks and two signature lines. PDF can be shared through Android's share sheet and sent to WhatsApp if installed. Android Print Framework is supported.

## Branding
Default company name: PERFECT PRINTING HOUSE.
Phone and address are editable in Settings.
