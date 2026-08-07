# Database Design

## Entity 1: User

Stores user account information.

Attributes:

- User ID
- Full Name
- Email
- Password
- Profile Picture (optional)

---

## Entity 2: Clothing Item

Stores all wardrobe items.

Attributes:

- Clothing ID
- User ID
- Clothing Name
- Category
- Color
- Brand
- Season
- Occasion
- Purchase Date
- Purchase Price
- Number of Times Worn
- Clothing Image

---

## Entity 3: Outfit

Stores outfits created by users.

Attributes:

- Outfit ID
- User ID
- Outfit Name
- Occasion
- Date Created

---

## Relationships

One User

↓

can own

↓

Many Clothing Items

One User

↓

can create

↓

Many Outfits

One Outfit

↓

contains

↓

Multiple Clothing Items
