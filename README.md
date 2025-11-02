# Ropstam-Test-Assessment
there are two theme files, one store is showing price getting from the metafield Pricing Table and one from the Variants price from beckend
## Installation

1. **Add metafield to product:**
   - Name: Width Options
   - Key: custom.width_options  
   - Type: JSON
   - Value: {"46":1,"66":2,"90":2,"112":3,"132":3}

2. **Replace variant_picker block in main-product.liquid**
   - Find: {%- when 'variant_picker' -%}
   - Replace with provided code

3. **Create product variants:**
   - Option 1: Fabric Panel (1, 2, 3 panels)
   - Option 2: Drop (54", 72", 90", 108")

4. **Set variant prices in Shopify Admin**

5. **Assign images to variants**

## How It Works

Customer selects Width (46") → System calculates 1 panel needed
Customer selects Drop (54") → System finds variant "1 panel / 54""
Price displayed from variant → Rs.20 (first variant)
Properties hidden from customer (fabric panel details hidden using _Fabric-panel in main-cart-items.liquid), visible to admin
