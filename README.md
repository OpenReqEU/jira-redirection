# OpenReq Issue Link Map - Jira Redirection Plugin

This web application was created as a result of the OpenReq project funded by the European Union Horizon 2020 Research and Innovation programme under grant agreement No 732463.

This jira plugin creates a new section in the View Issue Page that contains a link which redirects the user to the corresponding issue link map in the OpenReq Issue Link Map. 

## Technical description
### Technologies used
- Mockito
- Google Gson
- javax
- atlassian

### Functionalities of the OpenReq Issue Link Map - Jira Redirection Plugin
The user gets redirected to the corresponding issue link map

### How to install
Create a .jar file 

_Eclipse_

https://help.eclipse.org/luna/index.jsp?topic=%2Forg.eclipse.jdt.doc.user%2Ftasks%2Ftasks-37.htm

_IntelliJ_

https://www.jetbrains.com/help/idea/packaging-a-module-into-a-jar-file.html

After creating the .jar file, go to "Add-ons" in your Jira's Setting and then "Manage Add-ons"
![ManageAddOns](https://github.com/OpenReqEU/jira-redirection/blob/master/pics/Jira-Manage-Addons.png)

### How to use
Click the link.

#### What does this application do?
Redirects the user to the OpenReq Issue Link Map.

## Notes for Developers
In order to use this plugin, the project [qthulhu](https://github.com/OpenReqEU/qthulhu) and all of uh's services have to be deployed and the corresponding parts of the code have to be changed. 

## How to contribute
See [OpenReq project contribution guidelines](https://github.com/OpenReqEU/OpenReq/blob/master/CONTRIBUTING.md). 

## License
Free use of this software is granted under the terms of the [EPL version 2 (EPL2.0)](https://www.eclipse.org/legal/epl-2.0/).
