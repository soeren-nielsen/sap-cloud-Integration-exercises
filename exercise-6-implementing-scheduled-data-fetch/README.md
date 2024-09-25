# Exercise 6: Implementing Scheduled Data Fetch

## Description:
Create an integration flow that fetches product data from the Northwind OData service on a scheduled basis. This will help users learn how to implement time-based triggers in integration flows.

### Steps:
1. **Set Up OData Connection:**
    - Create an OData connection to the Northwind service using the products endpoint:  
      `https://services.odata.org/V4/Northwind/Northwind.svc/Products`.

2. **Create Integration Flow:**
    - Create a new integration flow in SAP Cloud Integration.
    - Add a scheduler trigger to initiate the flow at specified intervals (e.g., every 5 minutes).

3. **Fetch Product Data:**
    - Add an OData receiver adapter to perform a GET request to fetch product data.

4. **Log Output:**
    - Add a log message step to output the fetched product data.
    - Ensure that timestamps are included in the logs for reference.

5. **Testing:**
    - Deploy the integration flow and monitor its execution over time.
    - Verify that data is fetched and logged correctly at each scheduled interval.

### Hints:
- Review the scheduling options available in SAP Cloud Integration to set appropriate intervals.
- Consider using a variable to store the last fetched timestamp for logging purposes.
- Test the flow to ensure it behaves as expected during multiple executions.

### Helpful Links:
- [OData Northwind Documentation](https://services.odata.org/V4/Northwind/Northwind.svc/)
- [SAP Cloud Integration Documentation](https://help.sap.com/docs/cloud-integration/sap-cloud-integration/sap-cloud-integration)
- [OData Basic Tutorial](https://www.odata.org/getting-started/basic-tutorial/)
