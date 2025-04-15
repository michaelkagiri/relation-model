Tables and Relationships Hotel

Hotel_Id (Primary Key) Hotel_Name Type

Type_Id (Primary Key) Type_Name Room

Room_Id (Primary Key) Floor Hotel_Id (Foreign Key referencing Hotel) Type_Id (Foreign Key referencing Type) Category

Category_Id (Primary Key) Category_Name Price Beds_numbers Room_Category (To handle the 1-to-N relationship between Room and Category)

Room_Id (Foreign Key referencing Room) Category_Id (Foreign Key referencing Category) Employee

Employee_Id (Primary Key) Employee_Name Employee_Speciality Hotel_Id (Foreign Key referencing Hotel) Leads (To handle the 1-to-N relationship where an employee leads others)

Leader_Id (Foreign Key referencing Employee) Employee_Id (Foreign Key referencing Employee) Explanation of Relationships Hotel to Room → 1:N (A hotel has multiple rooms, but a room belongs to one hotel). Hotel to Employee → 1:N (Each hotel has multiple employees, but an employee belongs to one hotel). Room to Type → 1:1 (Each room is associated with a specific type). Room to Category → 1:N (A room can belong to multiple categories). Employee leads Employees → 1:N (One employee can lead multiple employees).