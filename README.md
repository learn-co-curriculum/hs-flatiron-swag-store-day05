## Flatiron Swag Shop!
Let's set up a User class so people can start shopping! We need people to be able to sign up for the swag shop and start adding items to a shopping cart!

**Step 1** You know how for some online stores, you have to have an account to shop? Let's set up that part of our Swag Shop. We need to create a user model in `app/models/user.rb`. The User class should inherit from `ActiveRecord::Base`. 

**Step 2** We need to create a users table in the database with ID, name, and password attributes. You'll need to create a migration with `up` and `down` methods and then run that migration.

**Step 3** We need to create a Sign up page for our users to create an account. Create a new view with a sign-up form.

**Step 4** We need a controller action that processes the information from the sign-up form. This action should save the new user to the database.

**Step 5** Now we need to set up sessions in our controller to maintain the state of a logged in user.

**Step 6** You'll want to create a sign-in form that stores the `user_id` in the `session` hash.

**Step 7** If a user isn't signed in, we'll want to restrict them from seeing all the awesome swag. Remember, they can't buy it if they're not logged in.

**Step 8** Now we need users to be able to sign out. Let's create a sign out form that removes the `user_id` from the `session` hash.





