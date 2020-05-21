# How To tell If Record Is New Or Already Exists

The `new_record?` Active Record method can tell if a record is new or already exists

`User.new.new_record?` => returns `true`
`User.first.new_record?` => returns `false`

This is how Rails knows to use a POST request for new users and a PATCH for
editing users? when constructing a form using `form_with(@user)`.
So if it returns true, it uses POST, and PATCH if it returns false.
