# SAP Power Platform Integration Demo Solution

## Summary
This is a demo app to show how we can leverage Power Platform for SAP Integration.
This solution includes Canvas App, Power Automate Flow, Power Virtual Agent Chat bot and Custom Connector to connect SAP Demo Instance. The Canvas App lists all business partners, products and sales orders in SAP and allows users to create new sales orders. This demo can be further extended to other areas/data points in SAP.
 
In this app, we use 2 methods to connect to SAP.
* Inside the canvas app, we leveraged SAP ODATA custom connector that you can get from open source repository on GitHub to list Business Partners, Sales Orders and Product Data from SAP Gateway Demo System. Link: https://github.com/microsoft/PowerPlatformConnectors/tree/master/custom-connectors/SAP-ODATA-Demo 
* We built the Power Automate flow to create Sales Order and Sales Order Line Items in SAP using OData Connector which is still in Preview (as of April 18, 2022).
 
## Features
* Display list of Business Partners from SAP
* Display list of Sales Orders from SAP
* Display list of Products from SAP
* Allow adding Products to cart for check out
* Create new Sales order and Sales order line items in SAP
* PVA Bot to query Product Data from SAP System based on Product Code

## Prerequisite
You will need an SAP system for this integration. Here are the instructions to create an account on SAP Gateway Demo System (ES5):
https://developers.sap.com/tutorials/gateway-demo-signup.html

## Demo
[![SAP and Power Platform Integration Demo App Video](https://i.ytimg.com/vi/a1_kEUVjVYo/hqdefault.jpg)](https://www.youtube.com/watch?v=a1_kEUVjVYo)

## How to install the solution from App Source
[![How to install SAP and Power Platform Integration Demo App Video](https://i.ytimg.com/vi/z87QKX2JGIk/hqdefault.jpg)](https://www.youtube.com/watch?v=z87QKX2JGIk)

Support Doc: [How to install SAP and Power Platform Integration Demo App from App Source](/documents/HowToInstallSAPandPowerPlatformIntegrationDemoApp.pdf) 

## Demo Scenarios
### Scenario 1 
The organization has been using SAP as their core system for managing their financials & other operations. The sales team is currently overwhelmed with the number of new orders and needs a simpler way to create orders in SAP quickly from within Microsoft Teams as they receive orders from customers on phone or email.
![Scenario 1 Flow](/images/SAPPP-Scenario1.png)
 
### Scenario 2 
The products and pricing team wants to provide an easy way for sales and other teams to find product details like Price, Availability via virtual agent inside Microsoft Teams
![Scenario 2 Flow](/images/SAPPP-Scenario2.png) 

## Demo Screens
### Canvas App
List Sales Orders from SAP
![List Sales Orders from SAP](/images/CanvasApp-S2-ListSalesOrder.png)

List Products from SAP
![List Products from SAP](/images/CanvasApp-S3-ListProducts.png)

Create new Sales Order and Sales Order Line items in SAP system
![Create new Sales Order and Sales Order Line items in SAP system](/images/CanvasApp-S4-EditCartCheckOut.png)

Create new Sales Order and Sales Order Line items Flow
![Create new Sales Order and Sales Order Line items Flow](/images/Flow-S1-CreateSalesOrder.png)

Query Product Information Flow
![Query Product Information Flow](/images/Flow-S2-QueryProductInfo.png)

