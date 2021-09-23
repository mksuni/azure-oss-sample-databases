## Sample database from mysqltutorial.org 

## Sample database schema
The MySQL sample database schema consists of the following tables:

- Customers: stores customer’s data.
- Products: stores a list of scale model cars.
- ProductLines: stores a list of product line categories.
- Orders: stores sales orders placed by customers.
- OrderDetails: stores sales order line items for each sales order.
- Payments: stores payments made by customers based on their accounts.
- Employees: stores all employee information as well as the organization structure such as who reports to whom.
- Offices: stores sales office data.

## Installation for MySQL schema
1. Install [Azure CLI ](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli)
2. Create Azure database for MySQL Flexible server 
``` az mysql flexible-server create --name mydemoserver --pubic-access all ```
3. Import data using ```execute``` command. 
``` az mysql flexible-server execute -n mysqlservername -u adminuser -p "adminpassword" -f "path to mysqlsampledatabase.sql"```

## Installation for PostgreSQL schema
1. Install [Azure CLI ](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli)
2. Create Azure database for MySQL Flexible server 
``` az postgres flexible-server create --name mydemoserver --pubic-access all ```

3. Import data using ```execute``` command. 

``` az postgres flexible-server execute -n mysqlservername -u adminuser -p "adminpassword" -f "path to mysqlsampledatabase.sql" ```

## Schema ER diagram
![classic model ER diagram](./MySQL-Sample-Database-Schema.png)

