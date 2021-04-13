# Master Data Request

This business process allows Market Participants such as Energy Suppliers and Grid Access Providers to request and receive master data for a metering point registered in Green Energy Hub.  
Once such a request has passed validation, master data for the metering point will be made available through the [Post Office domain](https://github.com/Energinet-DataHub/geh-post-office) and under certain conditions information about the registered consumer(s) will be made available as well. If validation fails, a rejection will be made available.

For Energy Suppliers, this business process may be relevant during the quotation phase or once supply has commenced.

An Energy Supplier may only request master data information for [Accounting Points](https://github.com/Energinet-DataHub/green-energy-hub/tree/main/docs/dictionary-and-concepts/dictionary-metering.md). If the Accounting Point is active in a Parent-Child metering point structure, the data response contains a list of all Child Metering Points in this structure. If needed, the Energy Supplier may then subsequently request master data for those Child metering points.

Grid Access Providers are only allowed to request master data information for all types of Metering Points in their own Grid Areas.
