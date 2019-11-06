# CDS Sample Service

This CDS View is the basis for an OData service, used for testing OData stuff in NW ABAP. To be able to use this, you need

* an SAP NetWeaver ABAP system with support for CDS, like NetWeaver ABAP 7.52 Developer Edition
* ABAP in Eclipse (ADT)

# Introduction

The code and example follow closely SAP Help documentation and the included example on this topic. I only cut the additional documentation overhead and make the minimum needed information available here and in my blog (link following).

The task consists of 2 steps:

1.	Create CDS View
2.	Expose OData service

# Create CDS Data Source

In ADT, create a new CDS Data Definition.

* Name: ZDEMO_CDS_SalesOrderItem
* Description: List Reporting for Sales Order Item

Paste the following code in the new created file: https://github.com/tobiashofmann/cds_sample_service/blob/master/ZDEMO_CDS_SalesOrderItem

Save and activate the CDS View.


# Activate OData Service

Tx: /n/IWFND/MAINT_SERVICE
Click on Add Service

Search for services in the local system.

* System Alias: LOCAL
* Technical Service Name: ZDEMO_CDS_SALESORDERITEM_CDS

Click on Get Services. Select the service and click on Add selected Services
