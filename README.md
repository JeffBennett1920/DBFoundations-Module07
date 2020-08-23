#### DBFoundations-Module 07
###### Jeff Bennett IT FDN 130A  08/23/2000
## User Defined Functions(UDFs)

#######**When to Use a SQL UDF**#######
UDFs are used to craft a bespoke function not available in SQL Server as a built-in function, and particularly one which is expected to be used frequently. UDFs can be used to provide a single calculated value (for example, a total discounted order price quote) or a calculated value which can be applied to a value in each record of a table.  UDFs enable code to be written once and used often, either as a stand-alone function or as a component of a larger query or function.  
It should be noted, however, that in some cases a view with simpler syntax might be preferable to a given UDF, providing a more readily comprehensible or efficient alternative to a function.
