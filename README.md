Shopify collSplitter setup instructions

1. API key
  - Go to Shopify > Admin > Apps > Manage private apps > Create a new private app
    1. Set any name
    2. Set "Products, variants and collections" permissions to "Read and write"
    3. Set all other permissions to "no access"
    4. Save, then copy the generated "API key" and "Password"

2. Admin customer account
  - Register a new account directly on your site so you can set the password, which you cannot do from the admin panel
  - Go to Shopify > Admin > Customers
    - Find the new account and add the tag "admin" (without quotes)

3. Liquid template file
  - Go to Shopify > Admin > Online Store > Themes
    1. Select the "Actions" drop-down on the current theme and pick "Edit code"
    2. Click on "Add a new template file" to create a new template for "page" called [anything]
    3. Copy the included file into the new template, configure the variables at the top of the script section (that API key), and save it

4. Page
  - Go to Shopify > Admin > Online Store > Pages > Add page
    1. Name it something easy to type
    2. Select the new template you just created in the "Template" drop-down on the right and save
    3. Set the visibility to public and leave it unlisted, as this uses the Shopify Admin API, which won't work from the page preview.

5. Navigate to the page after logging into the new customer account. It will not load anything otherwise.
