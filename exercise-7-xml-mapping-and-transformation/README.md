# Exercise: XML Mapping Using Graphical or XSLT Mapping

## Description:
Learn how to map an input XML structure to a desired output XML structure using either graphical mapping or XSLT mapping in SAP Cloud Integration.

### Steps:
1. **Set Up Integration Flow:**
    - Create a new integration flow in SAP Cloud Integration.

2. **Define Input XML Structure:**
    - Use the provided sample input XML file (`sample-input.xml`) which contains product data.
    - The input structure is defined in the `input.xsd` file.

3. **Message Mapping:**
    - Implement message mapping to transform the input XML into the desired output XML structure.
    - The output should include the following format:
   ```xml
   <ProductList>
       <ProductItem>
           <ProductID>1</ProductID>
           <ProductName>Coca-Cola</ProductName>
           <ProductCategory>Beverages</ProductCategory>
           <ProductPrice>18.00</ProductPrice>
       </ProductItem>
       <ProductItem>
           <ProductID>2</ProductID>
           <ProductName>Chang</ProductName>
           <ProductCategory>Beverages</ProductCategory>
           <ProductPrice>19.00</ProductPrice>
       </ProductItem>
   </ProductList>
   ```

4. **Choose Mapping Method:**

   - **Graphical Mapping:**
       - Use the graphical mapping editor to create the transformation by dragging and dropping elements from the input structure to the output structure.

   - **XSLT Mapping:**
       - Alternatively, create an XSLT mapping file to define the transformation logic.
       - The XSLT should transform the input XML into the desired output XML format.

### Log Output:

- Add a log message step to output the transformed XML.

### Testing:

- Deploy the integration flow and test it with the sample input XML file.
- Use the XML Validator step in SAP Cloud Integration to validate the output XML against the provided output XSD file.

### Hints:
- Review the input and output XSD files to understand the data structure and mapping requirements.
- Utilize the mapping documentation in SAP Cloud Integration for guidance on using graphical or XSLT mapping.
- Validate the output XML structure against the provided output XSD.

### Helpful Links:
- **SAP Cloud Integration Documentation:** [SAP Cloud Integration Documentation](https://help.sap.com/docs/cloud-integration/sap-cloud-integration/sap-cloud-integration)
