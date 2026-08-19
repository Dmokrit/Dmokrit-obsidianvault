The Database Case Proposal

Instructions: Select a **unique local organization** that you personally know or use (e.g., a specific neighborhood car repair shop, a niche university club, or a family-run craft business) that currently manage data using paper or Excel. This activity must be **hand-written** on **A4 size bond paper ( 1-2 pages only)**

Complete the following tasks:
1. Provide the organization's name and a 100-word description of how they currently handly data (e.g., "The local bookstore uses a shared Excel sheet for inventory and paper logs for customer orders").

	Organization Name: Dignos Boarding House
		Dignos Boarding House is a small family-run boarding house that accomodates students and workers. Currently, the owner manages information using paper records. Tenant information, room assignments, monthly rental payments, and contact details are written in a notebook. When a tenant pays rent, the owner manually updates the record. Room availability is also checked manually, as well as the water and the electricity bill. Maintainance concerns are usually communicated directly to the owner or via social media apps. This traditional system makes it difficult to handle the information efficiently as records may become disorganized which can affect the management and analyses of the boarding house's records.


2. Identify **three specific disadvantages** of their current "file-based" system (e.g., Data Redundancy, Program-Data Dependence, or Lack of Data Sharing) and explain how each specifically hurts their **business**.

	1. Program-Data Dependence
		The records depend on their existing format and method of organization. If the way the records are maintained changes, the owner may need to reorganize the files. This makes maintaining the boarding house records more difficult.
	2. Duplication of Data
		The same tenant information may be written in different records, such as tenant and payment records. If one record is updated while another is not, inconsistent information may occur.
	3. Limited Data Sharing
		Tenant, room, payment, and utility records are not centralized. The owner may need to check different records to find related information, making it slower to determine room availability, payment status, or expenses.


3. Identify one core entity (e.g., "Customer" or "Inventory Item") and create a **Metadata Table** for it. You must define at least **five attributes** with their Name, Type, Length, and Description (refer to sample in the Lecture Note 01).

| Data Item Name | Data Item Type | Data Item Length | Metadata Min. | Metadata Max. | Metadata Description                       | Metadata Source        |
| -------------- | -------------- | ---------------- | ------------- | ------------- | ------------------------------------------ | ---------------------- |
| Tenant ID      | Integer        | 5                | 1             | 99999         | Unique identification number of the tenant | Boarding House Records |
| Full Name      | Alphanumeric   | 50               |               |               | Complete name of the tenant                | Tenants                |
| Contact Number | Alphanumeric   | 15               |               |               | Tenant's mobile phone number               | Tenants                |
| Room Number    | Alphanumeric   | 10               |               |               | Number or identifier of the assigned room  | Boarding House Records |
| Monthly Rent   | Decimal        | 8                | 0.00          | 99999.99      | Monthly rental amount paid by the tenant   | Boarding House Records |
| Move-in Date   | Date           | 10               |               |               | Date when the tenant start renting         | Tenant                 |



4. List how the **nine components of the database environment** (refer to the Lecture Note 01) would specifically be realized in this business. You must name the actual **End User**s (e.g., "The Shop Manager") and the Application Programs (e.g., "A web-based order form") they would use.

	1. Data Modeling and Design Tools 
		A database modeling tool would be used to design the relationships between **Tenant, Room, Payment, Utility Bill, and Maintenance Request**.
	2. Repository
		Stores metadata about the boarding house database, such as data item names, types, lengths, and descriptions.
	3. Database Management System (DBMS)
		**MySQL** would manage the boarding house database and allow authorized users to store, update, and retrieve data.
	4. Database
		Stores information about **tenants, rooms, payments, utility bills, and maintenance requests**.
	5. Application Programs
		A **Boarding House Management System** would be used to register tenants, assign rooms, record payments, and monitor bills.
	6. User Interface
		A simple **web-based management interface** would allow the owner to add, search, and update records.
	7. Data/Database Administrators
		The **boarding house owner** would maintain the database and ensure that the records are accurate and consistent.
	8. System Developers
		A **software developer/programmer** would design and maintain the database and application programs.
	9. End Users
		The **boarding house owner/manager** would be the main end user. **Tenants** could also be end users if they are given access to their own room and payment information.

2. Describe the **Three-Schema Architecture** for this organization’s new database:
	- **External Schema:** Describe one specific **User View** (e.g., what a customer sees on an invoice).

		The boarding house owner would have a **Tenant and Payment View**. This view would display the tenant's name, room number, monthly rent, payment status, and payment date. A tenant's view could display only their own room and payment information. The external schema represents user views or subsets of the conceptual schema.
		
	- **Conceptual Schema:** Provide a high-level text description of the **entire structure** of the business's data.

		The database would contain entities such as **Tenant, Room, Payment, and Maintenance Request**. A tenant is assigned to a room and makes rental payments. Tenants may also submit maintenance requests. The entities would be related using appropriate keys. This provides a high-level representation of the organization's data structure, consistent with the conceptual schema described in the lecture note.


	- **Internal Schema:** Explain briefly how the data is **physically stored** in secondary memory.

		The database would be physically stored in secondary memory, such as an SSD or hard drive. The information would be organized into database tables and stored by the DBMS. This represents the logical and physical structures of the database under the internal schema.