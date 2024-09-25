# Exercise 2: Filtering Products by Category

## Description:
Modify the integration flow created in Exercise 1 to filter products by a specific category. This will help users understand how to apply query options in OData.

### Steps:
1. **Modify OData Connection:**
    - Use the same OData connection established in Exercise 1.

2. **Update Integration Flow:**
    - Change the OData receiver adapter configuration to include a filter.
    - Use the following OData query to filter products by category (e.g., `Beverages`):  
      `/Products?$filter=Category eq 'Beverages'`.

3. **Log Output:**
    - Add a log message step to output the filtered product data.

4. **Testing:**
    - Deploy the modified integration flow.
    - Run the flow and verify that only products in the specified category are returned.

### Hints:
- Review the OData documentation for more information on how to construct queries.
- Test the filter query directly in a web browser to see the expected results before implementing it in SAP Cloud Integration.

### Helpful Links:
- [OData Northwind Documentation](https://services.odata.org/V4/Northwind/Northwind.svc/)
- [SAP Cloud Integration Documentation](https://help.sap.com/viewer/product/SAP_CLOUD_PLATFORM_INTEGRATION/)
- [OData Basic Tutorial](https://www.odata.org/getting-started/basic-tutorial/)