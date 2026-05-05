# Design: Add to Cart

*Linked issues: #1, #2*

## Sketch

```
[Apple - $2]   [Add to Cart]
[Bread - $4]   [Add to Cart]

   Cart: 2 items
```

## Data flow

- **Input:** user clicks the Add to Cart button on a product
- **Process:** the product ID is added to a cart array, and the array length is recalculated
- **Output:** the cart count number on screen updates to the new total

## Design decisions

- Cart stored in a JavaScript array (not localStorage — out of scope for v1)
- Cart count shown as plain digits, no styling required
- One Add to Cart button per product (no quantity selector)
- Click adds 1 each time; no decrement option in this version
