# Exercise 5: Error Handling in Integration Flows

- **GitHub-friendly Name:** `error-handling-in-integration-flows`
- **Real Name:** Error Handling in Integration Flows

## Description:
Implement error handling within an integration flow that fetches product data from the Northwind OData service. This exercise will help users understand how to manage exceptions effectively.

### Steps:
1. **Set Up OData Connection:**
    - Create an OData connection to the Northwind service using the products endpoint:  
      `https://services.odata.org/V4/Northwind/Northwind.svc/Products`.

2. **Create Integration Flow:**
    - Create a new integration flow in SAP Cloud Integration to fetch product data.
    - Add an OData receiver adapter to perform a GET request.

3. **Implement Error Handling:**
    - Use a process step to define error handling for the integration flow.
    - Configure error handling to log any exceptions that occur during the fetching of data.
    - Add a log message step to capture and log error details for analysis.

4. **Testing:**
    - Deploy the integration flow and simulate a scenario where the OData service is temporarily unavailable by changing the endpoint to a non-existent one, such as:  
      `https://services.odata.org/V4/Northwind/Northwind.svc/InvalidEndpoint`.
    - Verify that the error handling mechanism logs the appropriate messages.

### Hints:
- Familiarize yourself with the built-in error handling options in SAP Cloud Integration.
- Consider using a custom error message format to improve log readability.
- Test the error handling by deliberately causing an error in the integration flow.

### Helpful Links:
- [OData Northwind Documentation](https://services.odata.org/V4/Northwind/Northwind.svc/)
- [SAP Cloud Integration Documentation](https://help.sap.com/viewer/product/SAP_CLOUD_PLATFORM_INTEGRATION/)
- [OData Basic Tutorial](https://www.odata.org/getting-started/basic-tutorial/)
