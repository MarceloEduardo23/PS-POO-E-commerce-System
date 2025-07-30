# Class structure

# 1 - Class '**Users**'
This is the base class representing a customer of the store.

# 2 - Class '**Admin**' (inherits from user)
An Admin is a special type of User with elevated privileges.

# 3 - Class '**Product**'
Stores all data related to a single product.

# 4 - Class '**Shopping Cart**'
A temporary class that holds items for a user who has not yet completed a purchase.

# 5 - Class '**Order**'
A crucial class representing the confirmation of a purchase. It acts as a snapshot of the shopping cart at the moment of checkout.

# 9 - Class '**Payment**'
This class is associated with an Order to process the financial transaction.
