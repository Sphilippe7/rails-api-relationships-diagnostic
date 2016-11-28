# Rails API Relationships Diagnostic

Place your responses inside the fenced code-blocks where indivated by comments.

1.  Describe a reason why a join tables may be valuable.

```sh
a join table is good for having a many to many relationship between objects.
```

1.  Provide a database table structure and explain the Entity Relationship that
describes a many-to-many relationship for `Profiles`, `Movies` and `Favorites`
(Think of Netflix). A `Profile` has a `given_name`, `surname` and `email` and a
`Movies` have `title`, `release_date`, and `length` and `Favorites` would be the
join table with references to `Movies` and `Profiles`.

```sh

```

1.  For the above example, what needs to be added to the Model files?

```rb
class Profile < ActiveRecord::Base
    def Profiles(:given_name , :surname , :email)


  end
end
```

```rb
class Movie < ActiveRecord::Base
end
```

```rb
class Favorite < ActiveRecord::Base
end
```

1.  What is the purpose of a serializer? What would our `Profile` serializer look
like to show all movies favorited by a profile on
`http://localhost:3000/profiles/1`

```sh
  # < Your Response Here >
```

```rb
class ProfileSerializer < ActiveModel::Serializer
end
```

1.  What would the command be to _scaffold_ out a **join table** for Favorites from
the above `Movies` and `Profiles`.

```sh
  # < Your Response Here >
```

1.  What is `Dependent: Destroy` and where/why would we use it?

```sh
dependent: destroy would be used in the command line and you would use it to remove
that object from the table.
```

1.  Think of **ANY** example where you would have a one-to-many relationship as well
as a many-to-many relationship in an application. You only need to list the
description about the resources and how they relate to one another.

```sh
An example of a one to many relationship:

A SSN (Social Security Number) to a SSN (Social Security Number)
There are many SSN's distributed to many people but a person can only have one
SSN'.

An example of a many to many relationship:

Model of a car to car companies
There are sedans, coupes, jeeps, hatchback, and vans as car models for every
car brand/company.

```
