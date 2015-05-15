## Flatiron Swag Shop!

**If you've finished the previous days, you can ski p to step 12**

**Step 1** - Set up your app and MVC directories.

**Step 2** - Set up your public directory with directories for css, img and js.

**Step 3** - Set up your config.ru file.

**Step 4** - Set up a config directory and an environment.rb file - **don't forget your SQL database connection!** (Hint: It's totally okay to copy the environment.rb file from your Fwitter project.)

**Step 5** - Set up your Gemfile with all of your gems - don't forget activerecord and sqlite3 (totally okay to copy from Fwitter again!)

**Step 6** - Set up your Rakefile (copy that Fwitter!)

**Step 7** - Now for the MVC. We're going to start with one model/table for Items with the following attributes/columns:

```ruby
:name
:image_url 
:price
:count
```

Create an `item.rb` file with an Item class - **don't forget to inherit from ActiveRecord::Base**. If you already created `item.rb` last week make sure to delete (or comment out) everything inside of the Item class - you don't need it and it might conflict with ActiveRecord.

**Step 8** - Create a migration for the items table `rake db:create_migration NAME="create_items"` and get in there to set up your `up` and `down` methods. (Look at your Fwitter migration!). Don't forget to run your migration with `rake db:migrate` when you are done! 

**Step 9** - Let's add some items to our database! Boot up `tux` in your terminal and create some new items. Here are some image links that you can use:

+ [hat](https://s3.amazonaws.com/after-school-assets/flatiron-swag-store-lab/flatiron_hat.jpg)
+ [hoodie](https://s3.amazonaws.com/after-school-assets/flatiron-swag-store-lab/flatiron_hoodie.jpg)
+ [men's tee](https://s3.amazonaws.com/after-school-assets/flatiron-swag-store-lab/flatiron_tee_m.jpg)
+ [women's tee](https://s3.amazonaws.com/after-school-assets/flatiron-swag-store-lab/flatiron_tee_w.jpg)
+ [tote](https://s3.amazonaws.com/after-school-assets/flatiron-swag-store-lab/flatiron_tote.jpg)

You can set your own price and decide the count that you have in stock.

**Step 10** - We've got the M covered, now let's move onto the V. In your views directory create an `items.erb` file that will display all of the merch for our store - including each item's name, photo and price.

**Step 11** - Set up your `get '/items'` route to pull all of your items from the database and display them in your new `items.erb` template.

**Step 12** You know how for some online stores, you have to have an account to shop? Let's set up that part of our Swag Shop. We need to create a user model in `app/models/user.rb` that inherits from ActiveRecord::Base. 

**Step 13** We need to create a users table in the database with ID, name, and password attributes. You'll need to create a migration with `up` and `down` methods and then run that migration.

**Step 14** We need to create a Sign up page for our users to create an account. Create a new view with a sign-up form.

**Step 15** We need a controller action that processes the information from the form. This action should save the new user to the database.

**Step 16** Now we need to set up sessions in our controller to maintain the state of a logged in user.

**Step 17** You'll want to create a sign-in form that stores the `user_id` in the `session` hash.

**Step 18** If a user isn't signed in, we'll want to restrict them from seeing all the awesome swag. Remember, they can't buy it if they're not logged in.

**Step 19** Now we need users to be able to sign out. Let's create a sign out form that removes the `user_id` from the `session` hash.




