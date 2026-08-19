The Database Case Proposal

Instructions: Select a **unique local organization** that you personally know or use (e.g., a specific neighborhood car repair shop, a niche university club, or a family-run craft business) that currently manage data using paper or Excel. This activity must be **hand-written** on **A4 size bond paper ( 1-2 pages only)**

Complete the following tasks:
1. Provide the organization's name and a 100-word description of how they currently handly data (e.g., "The local bookstore uses a shared Excel sheet for inventory and paper logs for customer orders").

	Organization Name: Dignos Boarding House
		Dignos Boarding House is a small family-run boarding house that accomodates students and workers. Currently, the owner manages information using paper records. Tenant information, room assignments, monthly rental payments, and contact details are written in a notebook. When a tenant pays rent, the owner manually updates the record. Room availability is also checked manually, as well as the water and the electricity bill. Maintainance concerns are usually communicated directly to the owner or via social media apps. A traditional system that 


2. Identify **three specific disadvantages** of their current "file-based" system (e.g., Data Redundancy, Program-Data Dependence, or Lack of Data Sharing) and explain how each specifically hurts their **business**.

	1. Lack of Transparency
		asd
	2. Risk of Data Loss
	3. Data needs update overtime


3. Identify one core entity (e.g., "Customer" or "Inventory Item") and create a **Metadata Table** for it. You must define at least **five attributes** with their Name, Type, Length, and Description (refer to sample in the Lecture Note 01).

| Data Item Name | Data Item Type | Length | Description                                |
| -------------- | -------------- | ------ | ------------------------------------------ |
| Tenant ID      | Integer        | 5      | Unique identification number of the tenant |
| Full Name      | Alphanumeric   | 50     | Complete name of the tenant                |
| Contact Number | Alphanumeric   | 15     | Tenant's mobile phone number               |
| Room Number    | Alphanumeric   | 10     | Number or identifier of the assigned room  |
| Monthly Rent   | Decimal        | 8      | Monthly rental amount paid by the tenant   |
| Move-in Date   | Date           | 10     | Date when the tenant start renting         |



4. List how the **nine components of the database environment** (refer to the Lecture Note 01) would specifically be realized in this business. You must name the actual **End User**s (e.g., "The Shop Manager") and the Application Programs (e.g., "A web-based order form") they would use.

	1. Data Modeling and Design Tools - 
	2. Repository
	3. Database Management System (DBMS)
	4. Database
	5. Application Programs
	6. User Interface
	7. Data/Database Administrators
	8. System Developers
	9. End Users


5. Describe the **Three-Schema Architecture** for this organization’s new database:
	- **External Schema:** Describe one specific **User View** (e.g., what a customer sees on an invoice).

		The boarding house owner would have a **Tenant and Payment View**. This view would display the tenant's name, room number, monthly rent, payment status, and payment date. A tenant's view could display only their own room and payment information. The external schema represents user views or subsets of the conceptual schema.
		
	- **Conceptual Schema:** Provide a high-level text description of the **entire structure** of the business's data.

		The database would contain entities such as **Tenant, Room, Payment, and Maintenance Request**. A tenant is assigned to a room and makes rental payments. Tenants may also submit maintenance requests. The entities would be related using appropriate keys. This provides a high-level representation of the organization's data structure, consistent with the conceptual schema described in the lecture note.


	- **Internal Schema:** Explain briefly how the data is **physically stored** in secondary memory.

The database would be physically stored in secondary memory, such as an SSD or hard drive. The information would be organized into database tables and stored by the DBMS. This represents the logical and physical structures of the database under the internal schema.