# INTRODUCTION

The purpose of this document is to provide a detailed specification of the save user interface. 


## REQUIREMENTS

- "New User" button

    This button is required for user to add new user to database.

- "Hide Disabled User" checkbox
  
    On checked, if saved user's "Enabled" checkbox is not checked, disabled users will be hid in the table.
   
- "Save User" button
  
    This button is required for to save the new user's information and show it in the table.
  
- "Username" textbox
  
    Username of the user to be registered.
  
- "Display Name" textbox
  
    New user's display name.
  
- "Phone" textbox
  
    New user's phone number.
  
- "Email" textbox
  
    New user's email adress.
  
- "User Roles "selectbox
  
    New user's role will be selected.

  - Guest
  - Admin
  - Super Admin
  
- Enabled checkbox

## UI COMPONENTS
- Header
  - "New User" button
  - "Hide disabled User" checkbox 
  - "Save User" button
- Table
  - "ID" column
  - "User Name" column
  - "Email" column
  - "Enabled" column
- "New User" Form
  - "Username" textbox
  - "Display Name" textbox
  - "Phone" textbox
  - "Email" textbox
  - "User Roles" selectbox
  - "Enabled" checkbox

## BEHAVIOR OF THE PAGE
- When the page opened;
  - Header
  
    "New User" button and "hide disabled user" checkbox will be active. "Save User" button will ve deactive.

  - Table
  
    Table will be visible. All pre-saved enabled users in database will be shown.

  - New User Form

    This form won't be visible.
  
- "New User" button onclick;
  
  "New User" From visible will be active.

- "Hide disabled User" checkbox
  - If active: pre-saved users with enabled checkbox active will be shown in the table.
  - Else: All pre-saved users will be shown in the table.
  
- While filling the User Form
  - "Username" textbox will add Username data to database table. 
  - "Displayname" textbox will be equal to User Name column in the table.
  - "Phone" and "Email" textboxes will be added to required column in database.
  - "User Roles" selectbox will choose the user's role that already defined in code side.
    - Guest
    - Admin
    - SuperAdmin
  - "Enabled" checkbox defines if this user is enabled or not. If not, saved user won't be shown in table untill hide disabled user checkbox is deactive.

- After all textboxes filled "Save User" button will be active.
  - "Save User" button onclick: related textboxes will be added to database.
  - Table will be refreshed. 


## AT THE BEGINNING
When the user opens the save user interface, a page opens where the user can register or view previously registered users.The user must press the new user button to add a new user. In addition, the "Save User" button will not be active until you fill in the information completely.
The user have the option to see all users or just the enabled ones by "Hide disabled User" checkbox.
