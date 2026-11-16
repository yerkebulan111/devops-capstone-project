# User Stories

## Epic: Product Catalog Management

### User Story 1: Create a Product
As a Product Store Owner,  
I want to be able to create new products in the catalog,  
So that I can keep track of new inventory.

**Acceptance Criteria:**
- Given a product payload with valid attributes (name, description, price, available, category), when a POST request is sent to `/products`, then the product is created with a unique ID and a 201 Created status code.

---

### User Story 2: Read a Product
As a Product Store Owner,  
I want to be able to retrieve a product by its ID,  
So that I can view its details.

**Acceptance Criteria:**
- Given an existing product ID, when a GET request is sent to `/products/{product_id}`, then the product details are returned with a 200 OK status code.

---

### User Story 3: Update a Product
As a Product Store Owner,  
I want to be able to update an existing product's information,  
So that I can keep inventory details accurate.

**Acceptance Criteria:**
- Given an existing product ID and updated fields, when a PUT request is sent to `/products/{product_id}`, then the product is updated and returned with a 200 OK status code.

---

### User Story 4: Delete a Product
As a Product Store Owner,  
I want to be able to delete a product from the catalog,  
So that I can remove discontinued items.

**Acceptance Criteria:**
- Given an existing product ID, when a DELETE request is sent to `/products/{product_id}`, then the product is removed and a 204 No Content status code is returned.

---

### User Story 5: List All Products
As a Product Store Owner,  
I want to be able to list all products in the catalog,  
So that I can review my complete inventory.

**Acceptance Criteria:**
- When a GET request is sent to `/products`, a list of all products in the system is returned with a 200 OK status code.
