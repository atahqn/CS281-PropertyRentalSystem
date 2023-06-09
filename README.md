# CS281 Property Management System - Code Documentation

The final provided code outlines the workflow for the CS281 Property Management System. It operates on a database named 'CS281.db' and utilizes PySimpleGUI for its graphical interface.

### Key Functions:

1. `login_window()`: Creates a login window for the user to input their credentials.

2. `window_owner()`, `window_admin()`, `window_customer()`: Create the corresponding windows for owners, admins, and customers respectively.

3. `window_property()`, `view_owner()`, `view_customer()`: These functions display the information for a particular property, owner, or customer.

4. `window_change_property()`, `window_change_evaluation()`: Create windows for changing property details and evaluations.

5. `change_evaluation_to_table()`: Updates the evaluation details in the database.

6. `window_book()`: Creates a window to handle property bookings.

7. `update_evaluation()`: Updates the property's evaluation in the database.

8. `update_book()`: Updates the booking information in the database.

9. `display_comments()`: Display comments for a property.

10. `see_bookings()`: Display the bookings of a property.

11. `sign_up_window()`: Create a sign-up window for new users.

12. `write_user_to_table()`: Writes new user details to the database.

13. `login_window()`: Creates a login window for the user to input their credentials.

14. `delete_property()`: Deletes a property from the database.

15. `window_add_property()`: Creates a window for adding a new property.

16. `write_property_to_table()`: Writes the new property details to the database.

17. `window_availability()`, `update_availability()`: Create windows and handle the updating of property availability.

### Workflow:

The script starts by connecting to the database 'CS281.db' and opening a login window. Once the user logs in, depending on their role (Owner, Admin, or Customer), they're directed to the respective windows where they can view properties, owners, or customers; change property or evaluation details; book properties; view bookings; and add or delete properties.

If a user is not yet registered, they can sign up through the `sign_up_window()`. After registration, their details are written to the database using `write_user_to_table()`.

Owners can update the availability of their properties with `window_availability()` and `update_availability()`. They can also add new properties using `window_add_property()` and `write_property_to_table()`, or delete existing ones with `delete_property()`.

At any point, users can log out and return to the login window.

If the window is closed, the program cleans up by closing any remaining open windows and commits any changes made to the database before closing the connection.

**Note**: This documentation is created based on the function names and code structure. Please ensure these functions are correctly implemented in your codebase. Always refer to your project's documentation for the most accurate information.
