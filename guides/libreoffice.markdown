---
layout: default
title: Setting up LibreOffice
---
# Setting up LibreOffice on your computer and connecting it to your MySQL database

First download LibreOffice from [its website](http://www.libreoffice.org) and install it on your computer.

LibreOffice needs Java runtime to function properly, so you may need to install Java as well. You can get a copy of Java Runtime Edition from [its website](http://java.com/en/download/mac_download.jsp?locale=en).

In order to connect LibreOffice Base to your MySQL server, you will need a JDBC connector. 

You can obtain your connector from [here](http://dev.mysql.com/downloads/connector/j/). Uncompress the file you have downloaded and keep it somewhere on your computer.

Now run LibreOffice and go to LibreOffice | Preferences menu. Select LibreOffice | Advanced in the sidebar. Click Class Path..., then click Add Archive... . Browse to the folder where you have saved the JDBC connector, and select the connector file (the one with .jar extension). You are done. Keep clicking OK until all dialogs are closed and you are back to the main window. You need to restart LibreOffice once for your modifications to take effect. 
