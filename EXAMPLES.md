# Chaufa Code Examples

This document provides functional code examples in Chaufa syntax, illustrating data entry, logging, inventory tables, and data calculations without external dependencies or graphic components.

## Example 1: Basic User Registration and System Logging

File: `register.cha`

```text
/=== USER REGISTRATION SYSTEM ===
:printspace

/Enter full name:
:inserttext
:saveinfo
:savevar name

/Enter department:
:inserttext
:saveinfo
:savevar dept

:log User (:loadvar name) registered in department (:loadvar dept)
:printline

/Registration Summary:
/Name: (:loadvar name)
/Department: (:loadvar dept)
/Registered On: (:getdate) at (:gettime)

:printspace
/Audit Log:
:showlog

:endprogram
```

## Example 2: Inventory Table Management and Filtering

File: `inventory.cha`

```text
/=== WAREHOUSE INVENTORY CONTROL ===
:createtable ID,Item,Quantity,Status
:insertrow 101,Storage_Rack,12,Available
:insertrow 102,Network_Cable,150,Available
:insertrow 103,Server_Unit,2,Low_Stock

:log Initialized inventory table with (:countrows) records.

/Current Inventory Output:
:showtable

:printspace
/Filtering Low Stock Items:
:filtertable Status == Low_Stock

:printspace
:endprogram
```

## Example 3: Numerical Processing with Lists

File: `metrics.cha`

```text
/=== BATCH METRICS PROCESSING ===
:printspace

:createlist batch_data
:addtolist batch_data 120
:addtolist batch_data 240
:addtolist batch_data 360

/Total processed entries: (:countlist batch_data)
/Combined batch sum: (:sumlist batch_data)

:log Processed (:countlist batch_data) batch records with total sum (:sumlist batch_data)

:printspace
/Session Event Log:
:showlog

:endprogram
```
