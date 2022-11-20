# Miscellanious stuff

- Add comments for posts
  - Create a comments table
    - Comments fields
      - Has body
      - Belongs to an author
      - Belongs to a post
    - Add foreign key constraints
      - For author
      - For post
      - Mention the database indexes that are created for foreign keys
  - Add a form before displaying comments for a post
  - Add endpoint `POST /posts/{posts:slug}/comments`
    - Name the controller and action `"PostCommentsController::store"`
      - Explain why to use this approach
  - Hide the form if there's no authenticated user

---

- Use Mailchimp's API for the "subscribe to newsletter" functionality
  - Check out mailchimp's API documentation for PHP
  - Tinker around with it
  - Setup the API keys
    - Show how to use the `".env"` and `".env.example"` files on these cases
    - Show how to make use of `"config()"`
  - Add endpoint for subscribing to newsletter
    - Add try/catch for possible errors, such as
      - Such as a gibberish email provided
- Create a newsletter service
  - Has a subscribe method that accepts an email
