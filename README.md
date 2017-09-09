# Inventory-Data-Warehouse
The Inventory Data Warehouse provides data to answer business intelligence questions about inventory transaction cycles. The data warehouse was created by a former database student for an independent study project. The former student had a strong background about inventory transaction cycles through his work with the OneWorld product of the former J.D. Edwards (now part of Oracle). 


# Inventory Transaction Cycles
Inventory that is bought, sold, consumed, and produced is the heart of any manufacturing and/or distribution company.  Inventory transactions are frequent and commonplace.  The volume and significance of inventory transactions make them important in a data warehouse design.
Because inventory management is a common and important yet difficult activity in many organizations, ERP vendors have developed Enterprise Resource Management (ERP) software to provide software support. Typically, ERP software provides modules related to Manufacturing, Distribution/Logistics, Financials, and HR/Payroll.  Inventory is at the heart of the Manufacturing and Distribution/Logistics modules.  The work order, sales, and purchase life cycles affect the perpetual inventory balance as shown in Figure 1. In addition, inventory transactions including adjustments, transfers, issues, and reclassifications affect the perpetual inventory balance.


# Snowflake Schema Description
To support reporting about inventory management, Figure 2 shows a snowflake schema for the perpetual inventory balance. The snowflake schema provides a template that can be customized to individual organizations. Dimension entity types such as Addr_Cat_Code1 allow an organization to customize the design to specific requirements. The fact entity type, Inventory_Fact, contains several measures along with relationships to associated dimension entity types. Several dimension entity types are related directly to the Inventory_Fact entity type. Other dimension entity types such as Item_Cat_Code1 are indirectly related to the Inventory_Fact entity type. 
