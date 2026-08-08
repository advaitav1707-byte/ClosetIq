# Database Design

## Entity 1: User

Stores user account and basic profile information.

Attributes:

- User ID
- Full Name
- Email
- Password
- Profile Picture (optional)

---

## Entity 2: Fashion Item

Stores every fashion item in the user's personal collection.

A fashion item can belong to different categories such as clothing, jewelry, footwear, or accessories.

Attributes:

- Fashion Item ID
- User ID
- Item Name
- Category
- Subcategory
- Color
- Brand
- Material
- Occasion
- Season
- Purchase Date
- Purchase Price
- Number of Times Worn
- Image

### Main Categories

- Clothing
- Jewelry
- Footwear
- Accessories

### Examples

Clothing → Shirt, Jeans, Dress, Jacket

Jewelry → Earrings, Necklace, Ring, Bracelet, Watch

Footwear → Sneakers, Heels, Flats, Boots, Sandals

Accessories → Bags, Belts, Sunglasses, Scarves, Hair Accessories

---

## Entity 3: Outfit

Stores outfits created by users.

Attributes:

- Outfit ID
- User ID
- Outfit Name
- Occasion
- Date Created
- Style/Vibe

Examples of Style/Vibe:

- Casual
- Minimal
- Formal
- Streetwear
- Elegant
- Party

---

## Entity 4: Outfit Items

Connects fashion items with outfits.

Attributes:

- Outfit Item ID
- Outfit ID
- Fashion Item ID

This allows one outfit to contain multiple fashion items.

For example:

An outfit can contain:

- White Shirt
- Blue Jeans
- Gold Earrings
- White Sneakers
- Black Bag

---

## Relationships

### User → Fashion Items

One User can own many Fashion Items.

**Relationship: 1 : Many**

---

### User → Outfits

One User can create many Outfits.

**Relationship: 1 : Many**

---

### Outfit → Fashion Items

One Outfit can contain many Fashion Items.

One Fashion Item can also be used in many Outfits.

**Relationship: Many : Many**

This relationship is managed through the Outfit Items entity.

---

## AI and Personalization Data

ClosetIQ can use information from the user's fashion items and outfit history to understand their preferences.

Potential data points include:

- Frequently worn colors
- Frequently worn categories
- Preferred brands
- Most-used fashion items
- Least-used fashion items
- Frequently combined items
- Preferred outfit styles
- Shopping patterns

This information can later be used for personalized outfit recommendations and smarter purchase suggestions.
