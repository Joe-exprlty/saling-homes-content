# Lofty Listing Search URL Reference Guide
### sellingpdxhomes.com City Pages

---

## Base URL Structure

```
https://www.sellingpdxhomes.com/cities/[PAGE-SLUG]?listingSource=all%20listings&condition=[ENCODED-JSON]&uiConfig=%7B%7D&zoom=15&page=1
```

The entire search is controlled by the `condition` parameter, which is a URL-encoded JSON object. Build the JSON first, then URL-encode it and insert it after `condition=`.

---

## Full Condition Object Reference

```json
{
  "location": {
    "city": ["City, ST"]
  },
  "propertytype": ["Single Family Home", "Condo", "Multi-Family", "Townhouse"],
  "listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"],
  "price": "MIN,MAX",
  "beds": "MIN,MAX",
  "baths": "MIN,MAX",
  "sqft": "MIN,MAX",
  "lotsize": "MIN,MAX",
  "yearbuilt": "MIN,MAX",
  "daysonsite": "MIN,MAX",
  "stories": "MIN,MAX",
  "garages": "MIN,MAX",
  "keyword": ["keyword1", "keyword2"]
}
```

---

## Value Format Rules

| Pattern | Meaning |
|---|---|
| `"300000,700000"` | Between min and max |
| `"300000,"` | Minimum only, no max |
| `",700000"` | Maximum only, no min |
| `","` | No filter applied |

This pattern applies consistently to ALL numeric fields: price, beds, baths, sqft, lotsize, yearbuilt, daysonsite, stories, and garages.

---

## Property Types

Use any combination in the array:

```
"Single Family Home"
"Condo"
"Multi-Family"
"Townhouse"
"Manufactured Home"
"Land"
"Commercial"
```

---

## Listing Status Options

```
"Active"
"Active Bumpable"
"BumpableBuyer"
"Pending"
"Sold"
```

For active listings, always include all three active statuses unless intentionally filtering:
```json
"listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"]
```

---

## Keywords

- Always include both capitalized and lowercase versions to cover case sensitivity
- Use an array for multiple keywords

```json
"keyword": ["Waterfront", "waterfront", "Pool", "pool"]
```

Common keyword examples:
```
"Waterfront" / "waterfront"
"Pool" / "pool"
"View" / "view"
"Corner Lot" / "corner lot"
"New Construction" / "new construction"
"Garage" / "garage"
"Basement" / "basement"
"ADU" / "adu"
```

---

## Common Search Examples

**Starter Homes Under $400k, 3+ Beds**
```json
{
  "location": {"city": ["Beaverton, OR"]},
  "propertytype": ["Single Family Home"],
  "listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"],
  "price": "100000,400000",
  "beds": "3,"
}
```

**New Listings in the Last 7 Days**
```json
{
  "location": {"city": ["Beaverton, OR"]},
  "propertytype": ["Single Family Home", "Condo", "Townhouse"],
  "listingstatus": ["Active"],
  "daysonsite": ",7"
}
```

**Single Story with Garage**
```json
{
  "location": {"city": ["Beaverton, OR"]},
  "propertytype": ["Single Family Home"],
  "listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"],
  "stories": ",1",
  "garages": "1,"
}
```

**Waterfront Properties**
```json
{
  "location": {"city": ["Beaverton, OR"]},
  "propertytype": ["Single Family Home", "Condo", "Multi-Family", "Townhouse"],
  "listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"],
  "keyword": ["Waterfront", "waterfront"]
}
```

**Condos and Townhouses Under $300k**
```json
{
  "location": {"city": ["Beaverton, OR"]},
  "propertytype": ["Condo", "Townhouse"],
  "listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"],
  "price": ",300000"
}
```

**Luxury Homes, 4+ Beds, 3+ Baths**
```json
{
  "location": {"city": ["Beaverton, OR"]},
  "propertytype": ["Single Family Home"],
  "listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"],
  "price": "700000,",
  "beds": "4,",
  "baths": "3,"
}
```

---

## How to Build a New Search URL

1. Write your condition JSON object using the fields above
2. URL-encode the entire JSON string (use any online JSON URL encoder)
3. Insert the encoded string into the base URL after `condition=`
4. Update `[PAGE-SLUG]` to match your city page slug

**Tip:** You can also build the search visually using the filters on the Lofty site, then copy the generated URL directly from the browser address bar and use it as your starting point.

---

## Real Example: Decoded vs Encoded

**Decoded (human-readable):**
```json
{
  "location": {"city": ["Beaverton, OR"]},
  "propertytype": ["Single Family Home", "Condo", "Multi-Family", "Townhouse"],
  "listingstatus": ["Active", "Active Bumpable", "BumpableBuyer"],
  "price": "100000,500000",
  "beds": "1,",
  "baths": "1,",
  "daysonsite": ",10",
  "stories": ",1",
  "keyword": ["Waterfront", "waterfront"]
}
```

**Encoded (ready to use in URL):**
```
%7B%22location%22%3A%7B%22city%22%3A%5B%22Beaverton%2C%20OR%22%5D%7D%2C%22propertytype%22%3A%5B%22Single%20Family%20Home%22%2C%22Condo%22%2C%22Multi-Family%22%2C%22Townhouse%22%5D%2C%22listingstatus%22%3A%5B%22Active%22%2C%22Active%20Bumpable%22%2C%22BumpableBuyer%22%5D%2C%22price%22%3A%22100000%2C500000%22%2C%22beds%22%3A%221%2C%22%2C%22baths%22%3A%221%2C%22%2C%22daysonsite%22%3A%22%2C10%22%2C%22stories%22%3A%22%2C1%22%2C%22keyword%22%3A%5B%22Waterfront%22%2C%22waterfront%22%5D%7D
```

---

*Reference guide for sellingpdxhomes.com city page development*
*Joe Saling | Saling Homes at eXp Realty | 503-910-7364*
