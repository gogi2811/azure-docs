---
author: msmimart
ms.service: active-directory-b2c
ms.subservice: B2C
ms.topic: include
ms.date: 06/11/2021
ms.author: mimart
# Used by Azure AD B2C app integration articles under "App integration".
---
1. Select the *my-api1* application you created to open its **Overview** page.

1. Under **Manage**, select **Expose an API**.
1. Next to **Application ID URI**, select the **Set** link. Replace the default value (GUID) with a unique name (for example, *tasks-api*), and then select  **Save**. 
 
   When your web application requests an access token for the web API, it should add this URI as the prefix for each scope that you define for the API.
1. Under **Scopes defined by this API**, select **Add a scope**.
1. To create a scope that defines read access to the API, enter the following values:

    a. **Scope name**: *tasks.read*  
    b. **Admin consent display name**: *Read access to tasks API*  
    c. **Admin consent description**: *Allows read access to the tasks API*

1. Select **Add scope**.

1. Select **Add a scope**, and then add a scope that defines write access to the API by entering the following values: 

    a. **Scope name**: *tasks.write*  
    b. **Admin consent display name**: *Write access to tasks API*  
    c. **Admin consent description**: *Allows write access to the tasks API*
1. Select **Add scope**.