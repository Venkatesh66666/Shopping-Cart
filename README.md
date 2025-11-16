# Online Shopping Cart (E-Commerce Website)

This is an E-Commerce Website build for selling of any electronics products online.

### About

In this project, a user can visit the website, register, and log in securely. They can browse all available products, apply category-based filters, search items, and add products to the cart. The user can also update the quantity (increase/decrease) in the cart. Once the cart is finalized, the user can move to checkout and proceed with demo credit-card payment. After successful payment, the order is placed and will be visible under the orders section along with shipment status.

The **Admin panel** manages the entire store by adding, updating, or deleting products, monitoring inventory, and handling orders. Admin can update order shipping status and delivery status.


A major highlight of this project is **automated email communication**. Users receive emails during registration, order placement, order shipment, product restocking, and delivery confirmation. If a product is out of stock and later becomes available, the user will be notified via email automatically.

**Note:** The payment module is for demonstration only — no real payment gateway integration. Any card details will be accepted for demo purposes.

## Highlights :--

### Users will receive email notifications for the following actions:
- Successful Registration  
- Order Successfully Placed  
- Out-of-Stock Product Becomes Available  
- Successful Shipment & Delivery  

### Technologies used:-
1. Front-End Development:
- HTML
- CSS
- Javascript
- BootStrap

2. Back-End Development:
- Java (JDK 8+)
- JDBC
- Servlet
- JSP

3. Database:
- MySQL

### ================ Software And Tools Required ================
- : Git [https://www.youtube.com/watch?v=gv7VPQ4LZ7g]
- : Java JDK 8+ [https://www.youtube.com/watch?v=O9PWH9SeTTE]
- : Eclipse EE (Enterprise Edition) [https://www.youtube.com/watch?v=8aDsEV7txXE]
- : Apache Maven [https://www.youtube.com/watch?v=jd2zx3dLjuw]
- : Tomcat v8.0+ [https://youtu.be/mLFPodZO8Iw?t=903]
- : MySQL Server [https://www.youtube.com/watch?v=Ydh5jYA6Frs]
- : MySQL Workbench [https://www.youtube.com/watch?v=t79oCeTXHwg]

### ================= Dummy Database Initialization =================
STEP 1: Open MySQL Command Prompt or MySQL Workbench

STEP 2: Login to the administrator user of MySql:
	 ```mysql -u <username> -p``` (Enter Password if asked)

STEP 3: Copy paste and execute the MySQL Query from the following file:-
- Run the Sql Query From this file: [databases/mysql_query.sql](./databases/mysql_query.sql)

### ======GENERATING GMAIL APP PASSWORD [For Mailing Functionalities]========
Step 1: Create a gmail account or login to existing account in any browser

Step 2 : Go to [https://myaccount.google.com/security](https://myaccount.google.com/security) and check if 2 step verifications is enabled or not, enable it if not enabled

Step 3: Go to [https://myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords) and enter password if asked

Step 4: In Select an App Section: select Other (custom name) => enter "Ellison Electronics" => Generate

Step 5: After that it will generate 16 digits app password which you need to copy and save for future configurations.

Step 6: Done : Now continue to importing the project. [Don't share the above password generated to anyone]

### ========== Importing and Running The Project Through Eclipse EE ==========

Step 1: Open Eclipse Enterprise Edition. [Install, if not already installed.]

Step 2: Click On File > Import > Git > Projects From Git > Clone Uri > Paste The Repository Url as: ```https://github.com/Venkatesh66666/Shopping-Cart.git```> Select master Branch > Next > Next > Finish.

Step 3: Go inside ```Java Resources > src > application.properties``` and update the values as below:
- a) Update value for db.username and db.password according to your installed mysql credentials.
- b) Update value for mailer.email and mailer.password, with the same email and app password that you generated earlier in above section [ NOTE:Actual gmail password will not work]

Step 4: Right Click on Project > Run as > Maven Build > In the goals field enter "clean install" > apply > run

Step 5: Right Click On Project > Build Path > Configure Build Path > Libraries > Remove and Update Any Libraries if Red Mark Exists > Finish.

Step 6: Right Click on Project > maven > update project > select force update > apply > close

Step 7: Tomcat Configurations:
- If Tomcat Server is not configured in Eclipse :
	-  Right Click On Project > Run As > Run On Server > Manually Define a new server > Select server type > select Tomcat v8.0+ > (Select Tomcat V8.0+ Installation Location If Asked) > Next > Add the current project > Finish.

- Else If Tomcat Server is already configured in Eclipse:
	- Right Click On Project > Run As > Run On Server > Select Tomcat Version > Next > Add the project > Finish.
		<p align='center'>or</p>
	- You can directly goto server tab, select the tomcat server and use the debug or run button to start the previously ran project

Step 8: Check Running The Site At  [http://localhost:8080/shopping-cart/](http://localhost:8080/shopping-cart/)

Step 9:  [To Change the Port, if getting error like 'port already in use'] Open The Server Tab > Double Click On Tomcat Server > Ports > Change The Port Number For Http/1.1 To 8083 > Close And Save. Now Start and you can access the project on [http://localhost:8083/shopping-cart/](http://localhost:8083/shopping-cart/)

Step 10: Default Username And Password For Admin Is "admin@gmail.com" And "admin"

Step 11: The default Username And Password For User Is "guest@gmail.com" And "guest"

## FAQ
**Question:1** Unable to Connect to Database?

**Answer:** Please check you have installed the mysql correctly and have updated the correct db details in application.properties file. Also you can try doing maven clean install and force update the project and restart.
<hr>

Note:- This is a Sample Project for learning purpose, we have not much considered of web security.

#### Some Screenshots for the project:
- Home Page
<img width="1920" height="1008" alt="Home Page" src="https://github.com/user-attachments/assets/faa52984-7024-4ebb-8ac8-52a18e966bc5" />

- Login Page
<img width="1920" height="1008" alt="Login Page" src="https://github.com/user-attachments/assets/09e71eb1-a3e4-4d18-be37-bb4111809918" />

- Register Page
<img width="1920" height="1008" alt="Register Page" src="https://github.com/user-attachments/assets/a4fdd8f6-9a7f-4042-82e0-33b20aa273f5" />

- Category Wise Product Filter
<img width="1920" height="1008" alt="Category Wise Product Filter" src="https://github.com/user-attachments/assets/45190aca-f7bb-4b37-a470-bae9b570a188" />

- Cart Items
<img width="1920" height="1008" alt="Cart Items" src="https://github.com/user-attachments/assets/2a8cc8ea-43e3-47e3-9e50-c6b2a9940861" />

- Credit Card Payment
<img width="1920" height="1008" alt="Credit Card Payment" src="https://github.com/user-attachments/assets/59538974-3869-42a2-9b96-236290b9277e" />

- Order Details & Status
<img width="1920" height="1008" alt="Order Details   Status" src="https://github.com/user-attachments/assets/fc83e23d-fb0a-4d31-a38e-88a7ab1cb51d" />

- User Profile
<img width="1920" height="1008" alt="User Profile" src="https://github.com/user-attachments/assets/7ab54758-96b1-4806-943f-7a1966c62097" />

- Admin Home
<img width="1920" height="1008" alt="Admin Home" src="https://github.com/user-attachments/assets/f956bf5d-a458-43c0-8f0f-028c7a9d2dc1" />

- Stock Items
<img width="1920" height="1008" alt="Stock Items" src="https://github.com/user-attachments/assets/e3922d13-bd25-4d8d-863f-6ba9c986fd1b" />

- Shipped Items
<img width="1920" height="1008" alt="Shipped Items" src="https://github.com/user-attachments/assets/416e68ef-0070-458f-8fba-483899daff40" />

- Recent Orders yet to be shipped
<img width="1920" height="1008" alt="Recent Orders yet to be shipped" src="https://github.com/user-attachments/assets/39752907-6809-4a80-851c-272f87a709b8" />

- Add Product to the stock
<img width="1920" height="1008" alt="Add Product to the stock" src="https://github.com/user-attachments/assets/91f76329-c372-4b45-ab4c-433d420c58df" />

- Remove Product from the stock
<img width="1920" height="1008" alt="Remove Product from the stock" src="https://github.com/user-attachments/assets/93438a22-dc10-41ce-b851-1e9df8ab8eaa" />

- Update the stock item
<img width="1055" height="551" alt="Update the stock item" src="https://github.com/user-attachments/assets/fc8b5030-6bcd-412c-b0e7-2288cfe17d2d" />

- Sample Email for order placed
<img width="598" height="418" alt="Sample Email for order placed" src="https://github.com/user-attachments/assets/336ac012-0b66-470a-a705-59495cc6f2ec" />

- Class Diagram
<img width="942" height="581" alt="Class Diagram" src="https://github.com/user-attachments/assets/fb33dd4d-0071-448a-9cd3-bdb808792d5c" />

#### "Suggestions and project improvement ideas are welcomed!"

<bold>Thanks a lot,</bold><br/>
                                                                                                        Project Leader<br/>
                                                                                                         <b>Venkatesh Choppadhandi</b>


