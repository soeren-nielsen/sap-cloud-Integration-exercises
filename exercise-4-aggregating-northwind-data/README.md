# Exercise 4: Aggregating Northwind Data

## Description:
Create an integration flow that aggregates data from multiple entities in the Northwind OData service, such as products and categories. This exercise will help users understand how to use mappings and transformations effectively.

### Steps:
1. **Set Up OData Connections:**
    - Create two OData connections in SAP Cloud Integration: one for the `Products` entity and one for the `Categories` entity.
    - Use the following endpoints:
        - Products: `https://services.odata.org/V4/Northwind/Northwind.svc/Products`
        - Categories: `https://services.odata.org/V4/Northwind/Northwind.svc/Categories`

2. **Create Integration Flow:**
    - Create a new integration flow in SAP Cloud Integration.
    - Add two OData receiver adapters: one for fetching products and another for fetching categories.

3. **Mapping and Transformation:**
    - Use a message mapping step to combine data from both sources into a single output format.
    - Include product details alongside their respective category names.

4. **Log Output:**
    - Add a log message step to output the aggregated results.
    - Ensure the output structure is clear and easy to read.

5. **Testing:**
    - Deploy the integration flow and run it.
    - Verify that the aggregated data is returned correctly.

### Hints:
- Use the OData `$expand` query option to retrieve related entity data in a single request.
- Check the structure of the response data in the OData service to facilitate proper mapping.
- Review the mapping documentation in SAP Cloud Integration for examples on how to structure your output.

### Helpful Links:
- [OData Northwind Documentation](https://services.odata.org/V4/Northwind/Northwind.svc/)
- [SAP Cloud Integration Documentation](https://help.sap.com/docs/cloud-integration/sap-cloud-integration/sap-cloud-integration)
- [OData Basic Tutorial](https://www.odata.org/getting-started/basic-tutorial/)
