---
title: Application Flow Chart
parent: CodeIgnitor Overview
permalink: /overview/appflowchart/ 
nav_order: 3
---

## **Application Flow Chart**

The following graphic illustrates how data flows throughout the system:

![Flow Chart](/Overview/appflowchart.jpg)


1. The index.php serves as the front controller, initializing the base resources needed to run CodeIgniter.
2. The Router examines the HTTP request to determine what should be done with it.
3. If a cache file exists, it is sent directly to the browser, bypassing the normal system execution.
4. Security. Before the application controller is loaded, the HTTP request and any user submitted data is filtered for security.
5. The Controller loads the model, core libraries, helpers, and any other resources needed to process the specific request.
6. The finalized View is rendered then sent to the web browser to be seen. If caching is enabled, the view is cached  first so that on subsequent requests it can be served.

