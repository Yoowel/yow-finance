-- [ Database Design ] --

[User]
PK id
name
email
password
created_at

[Wallet]
PK id
FK user_id -> User.id
name

[Transaction]
PK id
FK wallet_id -> Wallet.id
FK category_id -> Category.id
type
amount
date
note

[Category]
PK id
FK user_id -> User.id
name
