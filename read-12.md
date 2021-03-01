# EJS partials 

- EJS partials are used to help us to avoid repetition of the same code on several web pages.

- Includes are relative to the template with the include call. (This requires the 'filename' option.) For example if you have "./views/users.ejs" and "./views/user/show.ejs" you would use `<%- include('user/show'); %>`