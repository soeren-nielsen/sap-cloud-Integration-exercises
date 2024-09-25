# Exercise 3: Updating Northwind Products with Postman

## cription:
Ceate an integration flow that can receive product updates from an external system and update the Northwind OData service using Postman. This will provide insight into how to handle incoming data.

### Steps:
1. **Set Up Integration Flow:**
    - Create a new integration flow in SAP Cloud Integration.
    - Use the HTTP receiver adapter to set up an endpoint to receive incoming product updates.

2. **Configure Incoming Data:**
    - Define the expected JSON structure for product updates (e.g., product ID, name, price, and category).
    - Example JSON structure:
      ```json
      {
        "ProductID": 1,
        "ProductName": "New Product Name",
        "UnitPrice": 20.00,
        "Category": "Beverages"
      }
      ```

3. **Connect to OData Service:**
    - Use the HTTP sender adapter to connect to the Northwind OData service.
    - Configure a POST request to the `Products` entity to update product information.

4. **Testing with Postman:**
    - Deploy the integration flow and test it by sending a sample JSON payload to the integration flow's endpoint using Postman.
    - Verify that the product updates are reflected in the Northwind OData service.

### Hints:
- Make sure to set the `Content-Type` header to `application/json` in Postman when sending requests.
- Use the `PUT` method if you are updating an existing product, or `POST` if you are creating a new one.
- Check the response in Postman to confirm whether the update was successful and to catch any errors.

### Helpful Links:
-  [OData Northwind Documentation](https://services.odata.org/V4/Northwind/Northwind.svc/)
- [SAP Cloud Integration Documentation](https://help.sap.com/viewer/product/SAP_CLOUD_PLATFORM_INTEGRATION/)
