# Exercise 1: Fetching Data from Northwind OData Service

## Description:
Learn how to connect to the Northwind OData service and fetch data for products. The goal is to create an integration flow that retrieves product information and logs the results.

### Steps:
1. **Set Up OData Connection:**
    - Create a new OData connection in SAP Cloud Integration.
    - Use the following endpoint for the Northwind OData service:  
      [Northwind OData Service URL](https://services.odata.org/V4/Northwind/Northwind.svc/).

2. **Create Integration Flow:**
    - Create a new integration flow in SAP Cloud Integration.
    - Add an OData receiver adapter to connect to the Northwind service.
    - Configure the adapter to perform a GET request to the `Products` entity.

3. **Log Output:**
    - Add a log message step to output the response.

4. **Testing:**
    - Deploy the integration flow and run it.
    - Verify that the product data is returned correctly.

### Hints:
- Make sure to test the OData service in your browser to confirm that the endpoint is active and accessible.
- Use the `Trace` mode in your integration flow to step through the execution and identify any issues in real time.

### Helpful Links:
- [OData Northwind Documentation](https://services.odata.org/V4/Northwind/Northwind.svc/)
- [SAP Cloud Integration Documentation](https://help.sap.com/docs/cloud-integration/sap-cloud-integration/sap-cloud-integration)
