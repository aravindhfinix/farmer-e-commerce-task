### Admin Module
- **Admin Dashboard Functions:**
  - Login
  - Subadmin Management:
    - Create, List, Update, Get, Delete Subadmins

- **Farmer Management:**
  - Create, List, Update, Get Details, Delete Farmer
  - Search based on name, email, phone number, country name

- **Buyer Management:**
  - Approve/Reject Buyer KYC
  - List all buyers, List KYC pending buyers
  - Get Buyer details, Delete Buyer
  - Block and unblock buyer
  - Search based on name, email, phone number, country name

- **Category Management:**
  - Create, List, Get, Update, Delete Categories (if a category is deleted, all related products and farmer products should also be deleted)

- **Product Management:**
  - Create, List, Get, Update, Delete Products (related farmer products should also be deleted)
  - Approve/Reject Farmer Products
  - Image Upload API linked to create APIs

- **Shipment Management:**
  - Define available shipments from country to country

### Farmer Module
- **Farmer Dashboard Functions:**
  - Login
  - List Products (filter by category, search by name)
  - Get Product Details
  - Create Farmer-Product with quantity and price
  - List orders of his products

### Buyer Module
- **Buyer Dashboard Functions:**
  - Signup
  - KYC Upload

  - **After KYC Verification:**
    - Login
    - List Farmer Products (filter by category, search by product/farmer name)
    - Get Farmer Product details with price and quantity
    - Order available quantities of farmer products
    - Verify shipment availability between countries
    - Create orders and manage quantity deduction from farmer products
    - List his orders

### Common APIs
- **Image Upload API:** Uploads images and links them to various create APIs (e.g., product images, buyer profile pics, KYC)

### Emails
- **KYC:** KYC acceptance and rejection emails should be sent to the buyer.
- **Order:** If an order is placed by a buyer, both buyer and farmer should receive the order details via email.

### Additional Requirements
- **Authentication & Authorization:** Implement secure login mechanisms for each module.
- **Error Handling:** Manage errors such as shipment unavailability, validation errors, etc.
- **Search & Filtering:** Enable filtering and searching across various modules.
- **Joi Validations:** Ensure data validations across modules.
- **Notifications:** Implement notifications for actions like KYC approval, order status, etc.