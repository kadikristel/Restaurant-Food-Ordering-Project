# Restaurant Food Ordering App

A contactless web application designed for restaurants to facilitate food and drink ordering while ensuring compliance with GDPR regulations.

## Features

- **Contactless Ordering**: Customers can browse the menu and place orders without physical interaction.
- **Menu Management**: Upload and manage products with details like images, allergy information, and categories.
- **Order Management**: Staff can view, process, and manage incoming orders in real-time.
- **Contact Tracing**: Collects and securely stores customer information for 21 days to comply with privacy laws.
- **Accessibility**: Accessible via QR code or web address on smartphones, tablets, and computers.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/kadikristel/Restaurant-Food-Ordering-Project.git
   cd Restaurant-Food-Ordering-Project

## Documentation of use cases

UC1. Menu browsing with search:

    Description
    • This functionality allows the user to see a menu (list of products) provided by the restaurant. 
      The user can use search functions to filter the menu by various categories.
  
    Roles and permissions
    • No restrictions - every public user can use it.

    Business logic
    1. The user must be able to see a list of all products (menu) provided by the restaurant on the same page.
    2. The user must see the following information about every product:
      a. Product name
      b. Product price
      c. Product size (that may vary for different products)
      d. The user must see the label “Out of stock” if the product is not available.
    3. The list of products must be sorted by the product name.
    4. The user must be able to search products by their name - full-text search or partial search.
    5. The user must be able to filter the list of products by the following parameters:
      a. Category: Available categories are “Cold drinks”, “Desserts”, “Hot drinks”, “Pasta”, “Pizza”, “Salads”, 
          “Soups”, Starters”.
      b. Highlight: “House special”, “Spicy”, “Vegan”, “Vegetarian”.
      c. Allergy Information: “Eggs”, “Gluten”, “Milk”.
    6. The user must be able to apply one or multiple filtering parameters at the same time.

UC6. Product management

    Editing product details
    Description
    • This functionality allows the administrator to edit information of previosly added product.  

    Roles and permissions
    • Administrator - only administrator user must be able to access this functionalities. 
    
    Business logic
    1. The administrator must be able to edit product details by opening its in the menu. 
        The administrator must see “Edit” button, that must be hidden for other users.
    2. The administrator must be able to change all fields of the product.
        The fields and validations must work in the same way   as they described in the “Adding products” scenario.
    3. The administrator must be able to cancel editing by pressing “Cancel” button.
    4. The administrator must be able to save new data by pressing “Save” button. 
        After saving the administrator must be redirected to the Menu page.

    Deleting a product
    Description
    • This functionality allows the administrator to delete previosly added product.  
    
    Roles and permissions
    • Administrator - only administrator user must be able to access this functionalities. 

    Business logic
    1. The administrator must be able to delete product by opening its in the menu. 
        The administrator must see “Delete” button, that must be hidden for other users.
    2. The confirmation window must appear if administrator is pressing “Delete” button. 
        By confirming the action the administrator must be able to delete the product
        and it should not appear any more in the menu for other users.
  
