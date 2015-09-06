qbws
=========

This sample is a Node.js web service application that communicates with QuickBooks via QBWebConnector. The sample focuses primarily on demonstrating how to setup all web service web methods to run against QBWebConnector and does not focus on any particular use case. For simplicity, it sends three request XMLs: CustomerQuery, InvoiceQuery and BillQuery.

## Status ##

This project replicates the functionality of the ASP.NET web service found in the QBSDK. Unfortunately that means some things are hard coded that should not be, and other things are left unimplemented. Eventually, qbws will diverge from that C# example to serve less of an SDK example and more as a reliable utility.

## Usage ##

Install the package using `npm install qbws`. The following code is all you need to run the service:

    var qbws = require('qbws');
    qbws.run();

## Changelog ##

#### v0.2.0 ####
 - Functional port of [Intuit's WCWebService][1] provided in the QBSDK samples
 - Many things are hard coded for demonstration purposes:
   - Login credentials
   - Requests (CustomerQuery, InvoiceQuery, BillQuery)
   - Company file location

## Next Milestones ##
 - v0.2.1: Include documentation for all functions (likely using JSDoc)
 - v0.3.0: Conversion to Node.js utility


 [1]: https://developer-static.intuit.com/qbsdk-current/samples/readme.html#WCWebService%20(C#%20ASP.NET)%20(qbxml)%20(desktop)
 
