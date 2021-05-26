# Tutorial: How to Automatically Synchronize User Information from Azure AD via RICOH Cloud Service  
The user information to be registered via RICOH Cloud Service can be automatically obtained via synchronization with Azure AD. The information here explains the method for configuring this on Microsoft Azure Portal.  
## Creating an enterprise application   
1.  From Microsoft Azure Portal, open Azure Active Directory.  
1. On the left pane, click [Enterprise applications].  
![Application screen illustration](/img/dsgvwx8019.gif)  
1. Click [New application].  
![Application screen illustration](/img/dsgvwx8020.gif)  
1. Click [Create your own application].  
![Application screen illustration](/img/dsgvwx8021.gif)  
1.  In the "What's the name of your app?" field, enter an app name, and then click [Create].  
![Application screen illustration](/img/dsgvwx8022.gif)   
## Configuring the provisioning for the application created  
Before getting started, on the "Azure AD Automatic User Synchronization Settings" screen of the common management site for RICOH Cloud Service, check your endpoint, and then issue an access token. For information about operating the common management site, see the operating guide for the common management site.  
1. On the left pane, click [Provisioning].  
1. Click [Get started].  
![Application screen illustration](/img/dsgvwx8026.gif)  
1. Configure the following settings:  
    * Provisioning Mode: Automatic  
    * Tenant URL: From "Azure AD Automatic User Synchronization Settings" on the common management site, copy the address of "Endpoint", and then paste it here.  
    * Secret Token: Copy the access token issued via "Azure AD Automatic User Synchronization Settings" on the common management site, and then paste it here.  
![Application screen illustration](/img/dsgvwx3148.gif)  
1. Click [Test Connection].  
1.  If the test connection succeeds, click [Save].  

## Configuring the mapping for provisioning
1. Click [Mappings].  
1. Click [Provision Azure Active Directory Groups].  
![Application screen illustration](/img/dsgvwx8024.gif)   
1. Select "No" for "Enabled", and then click [Save].  
1. Click [Provision Azure Active Directory Users].  
![Application screen illustration](/img/dsgvwx8025.gif)  
1. Select "Yes" for "Enabled".  
1. On "Attribute Mappings", configure the mappings exactly as the attribute mappings shown on the Azure AD Automatic User Synchronization Settings screen.  
![Application screen illustration](/img/dsgvwx3151.gif) 
1. Click [Save].  

## Starting the provisioning
1. Click [Start Provisioning].  
For information about synchronization timings, see [Azure AD Specifications](https://docs.microsoft.com/en-us/azure/active-directory/app-provisioning/configure-automatic-user-provisioning-portal#provisioning-statusI).

## Reviewing the result of Azure AD automatic synchronization
1. Click [Provisioning Logs (Preview)] for the enterprise application created in the [Creating an enterprise application](#Creating-an-enterprise-application) step.  
