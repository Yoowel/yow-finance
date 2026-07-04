-- [ Database Design ] --

[User]
id
name
email
password
created_at

[Wallet]
id
user_id
name

[Transaction]
id
wallet_id
category_id
type
amount
date
note

[Category]
id
user_id
name
