## **Apex_basics**

### (Please see the Trailhead Challenges here: https://github.com/Lanigithub/Apex_Trailhead_Challenges )

#### 0. **Data Types Overview**

Apex supports various **data types**, including a data type specific to Salesforce—the **sObject data type**.
Apex supports the following data types:

#### * A **primitive**, such as an **Integer, Double, Long, Date, Datetime, String, ID, Boolean**, among others.
#### * An **sObject**, either as a **generic sObject** or as a **specific sObject**, such as an **Account, Contact, 
or MyCustomObject__c** (you’ll learn more about sObjects in a later unit.)
#### * A **collection**, including:
#### * A **list (or array) of primitives, sObjects, user defined objects, objects created from Apex classes, or collections
#### * A **set of primitives**
#### * A **map from a primitive to a primitive, sObject, or collection**
#### * A typed list of values, also known as an **enum**
#### * **User-defined Apex classes**
#### * **System-supplied Apex classes**

### 1. Collections:
(https://www.tutorialspoint.com/apex/apex_collections.htm#:~:text=A%20list%20should%20be%20declared%20with%20the%20keyword%20'List'.&text=Below%20is%20the%20list%20which,Value%20Of%20ListOfCities'%2BListOfCities)%3B)
#### **Lists:**
#### A list is an ordered collection of elements that are distinguished by their indices. List elements can be of any data type—primitive types, collections, sObjects, user-defined types, and built-in Apex types.
#### **Sets:**
#### A set is an unordered collection of elements that do not contain any duplicates. Set elements can be of any data type—primitive types, collections, sObjects, user-defined types, and built-in Apex types.
#### **Maps:**
#### A map is a collection of key-value pairs where each unique key maps to a single value. Keys and values can be any data type—primitive types, collections, sObjects, user-defined types, and built-in Apex types.
#### **arameterized Typing:**
#### Apex, in general, is a statically-typed programming language, which means users must specify the data type for a variable before that variable can be used.
 




### 2. **Apex_method 1**

####  In this Apex class we will learn how to declare a list and apply the basic list methods: **add(), addAll()**to add elements to an existing list,
####  **contains()** method  and **equal()** method for a boolean statement : true or false when compare two lists or checking existance of an element
####  **clone()** method to copy a list and **clear()** to delete all the elements of a list


### 3. **Apex method 2:**

####  *In this apex class you will learn about the following methods: 
#### **get(index):
#### ** getSObjectType(), indexOf( ), isEmpty(), remove(index), set(index,listElement) , size( ), sort( )


### **4. Apex method 3: Create a List with type Account to perform DML operations**

### **5. DML statement:**
(https://developer.salesforce.com/docs/atlas.en-us.apexref.meta/apexref/apex_dml_section.htm)

#### insert: The insert DML operation adds one or more sObjects, such as individual accounts or contacts, to your organization’s data. insert is analogous to the INSERT statement in SQL... Syntax : insert sObject;  insert sObject[]
insert sObject[]
#### update: The update DML operation modifies one or more existing sObject records, such as individual accounts or contacts, in your organization’s data. update is analogous to the UPDATE statement in SQL.   Syntax: update sObject;  update sObject[]
#### upsert: The upsert DML operation **_creates_** new records and **_updates_** sObject records within a single statement, using a specified field to determine the presence of existing objects, or the ID field if no field is specified.    upsert sObject​​[opt_field];  upsert sObject[]​​[opt_field]
#### delete: The delete DML operation deletes one or more existing sObject records, such as individual accounts or contacts, from your organization’s data. delete is analogous to the delete() statement in the SOAP API.
#### undelete: The undelete DML operation restores one or more existing sObject records, such as individual accounts or contacts, from your organization’s Recycle Bin. undelete is analogous to the UNDELETE statement in SQL.
#### merge: The merge statement merges up to three records of the same sObject type into one of the records, deleting the others, and re-parenting any related records.
#### Syntax
merge sObject sObject
merge sObject sObject[]

merge sObject ID

merge sObject ID[]

#### The first parameter represents the master record into which the other records are to be merged. The second parameter represents the one or two other records that should be merged and then deleted. You can pass these other records into the merge statement as a single sObject record or ID, or as a list of two sObject records or IDs.
#### Manipulate Records with DML
```
#### Learning Objectives
After completing this unit, you'll be able to:
Use DML to insert, update, and delete records.
Perform DML statements in bulk.
Use upsert to either insert or update a record.
Catch a DML Exception.
Use a Database method to insert new records with the partial success option and process the results.
Know when to use DML statements and when to use Database methods.
Perform DML operations on related records.
```



