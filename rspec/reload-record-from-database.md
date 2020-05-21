# Reload record from database in tests

`reload` to reload the object's values from the database and confirm
that they were successfully updated. For example: `@user.reload` when testing whether
an edit/PATCH was successful.
