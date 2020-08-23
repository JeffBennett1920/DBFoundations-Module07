###### Jeff Bennett IT FDN 130A  08/23/2000
## User Defined Functions(UDFs)

#### **Introduction**
Microsoft SQL Server not only provides built-in functions for commonly used aggregate, string manipulation, logic, date, formatting and other operations, but also enables users to construct their own User Defined Functions (UDFs) to encapsulate specialized and frequently used SQL code.  UDFs come in a variety of styles.

#### **When to Use a SQL UDF** 
UDFs are used to craft a bespoke function not available in SQL Server as a built-in function, and particularly one which is expected to be used frequently. UDFs can be used to provide a single calculated value (for example, a total discounted order price quote) or a calculated value which can be applied to a value in each record of a table.  UDFs enable code to be written once and used often, either as a stand-alone function or as a component of a larger query or function.  
It should be noted, however, that in some cases a view with simpler syntax might be preferable to a given UDF, providing a more readily comprehensible or efficient alternative to a function.

#### **Scalar, Inline and Multi-Statement Functions** 
Functions range from the simpler to the more complex variety:

##### Scalar Function -		
The scalar valued function *returns a single value* .  A scalar function can optionally take one or more parameters using the @variable syntax, make a calculation and return a single value.
    
##### Inline Table Function -		
The inline table valued function *returns a table*.  The Return Table As clauses are followed by a Return( ) statement which contains the main body of the function, including the Select, From, Order By and other statements within its parentheses.
  
##### Multi-Statement Function - 	
The multi-statement table valued function (MSTVF) *returns a table variable*.  The MSTVF returns a specifically defined table variable using the @variable syntax.  The columns of the function are then defined followed by the As clause.  MSTVFs typically use Begin and End syntax to bracket the multiple statements comprising the function’s main body, and then conclude with a Return statement.

#### **Summary** 
SQL Server User Defined Functions enable the user to encapsulate and reuse code which can be employed in specially designed functions, and then used as modular building blocks in larger functions and queries. 
