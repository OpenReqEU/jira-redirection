# OpenReq Issue Link Map - Jira Redirection Plugin

This repository is no longer maintained. This repository is archived for parties interested in the standalone functionality that this repo once offered. Now, the functionality has been moved to [OpenReq Issue Link Map](https://github.com/OpenReqEU/issuelinkmap-jira-plugin). For full details of capability and intended usage, please see [OpenReq Issue Link Map](https://github.com/OpenReqEU/issuelinkmap-jira-plugin).

This jira plugin was created as a result of the OpenReq project funded by the European Union Horizon 2020 Research and Innovation programme under grant agreement No 732463.

This jira plugin creates a new section in the View Issue Page that contains a link which redirects the user to the corresponding issue link map in the OpenReq Issue Link Map. In order for this to work, UH's services need to be deployed. To use the services in a different jira than Qt's jira, UH's services need to be adapted, otherwise there will be erros. Then inside the OpenReq Issue Link Map the endpoints to access the data need to be changed, as well as the adress in this plug-in to refer to the correct location of the OpenReq Issue Link Map.

## Technical description
### Technologies used
- Mockito
- Google Gson
- javax
- atlassian

### Sources
None

### Functionalities of the OpenReq Issue Link Map - Jira Redirection Plugin
The user gets redirected to the corresponding issue link map.

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
In order to use this plugin, the project [qthulhu](https://github.com/OpenReqEU/qthulhu) and all of UH's services have to be deployed and the corresponding parts of the code have to be changed. In this case the link has to be updated in here jira-redirection/src/main/resources/templates/jira-redirection.vm has to be updated accordingly. You also have to configure milla from UH to get your Jira data, and then qthulhu has to be updated to fetch the data from the correct source. As a list:
1. Adapt UH's services to work with your own jira
2. Change the endpoint addresses in the OpenReq Issue Link Map
3. Change the link in jira-redirection/src/main/resources/templates/jira-redirection.vm to the one where you are hosting the OpenReq Issue Link Map

## How to contribute
See [OpenReq project contribution guidelines](https://github.com/OpenReqEU/OpenReq/blob/master/CONTRIBUTING.md). 

## License
Free use of this software is granted under the terms of the [EPL version 2 (EPL2.0)](https://www.eclipse.org/legal/epl-2.0/).
