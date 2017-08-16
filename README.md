Provisioning a One-Directional E-mail System for MegaMaker

REQUIREMENTS

    * Allow the server to send an email to the user (does not need to be encrypted -- just a simple email)
    * Attach HTML format in the email
    * Can be written in any programming language 

FEATURES 

     * A backend service will perform one method: 
         1) Create New Password: Allow a user to create a new password and save it 

SOLVE THESE PROBLEMS 
     
    * How to establish a REST endpoint that allows user to reset password 
    * MAYBE use POST request to write to HTML page and give user a url that directs them to a services page to reset pw (our backend handles encryption)
    * MAYBE thru terminal be able to send email -> docker -> ubuntu -> linux shell 
    * MAYBE try node package: "mailgun-js" or sendgrid or mandrill (via youtube tutorials) 
    * Password will do a single-factor authentication -- instantiate a temporary code, pass it to the user, prompt them to enter it, and prompt them to re-create password 
    * On submit, database needs to be populated with new credentials but in encrypted form -- devs should not see it 
    * Number of https requests per session may need to be limited to prevent hacks
