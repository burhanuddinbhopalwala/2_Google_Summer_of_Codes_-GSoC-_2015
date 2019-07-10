#GSoC-2014-15-proposal #INCF-National-Node-of-Belgium #iRODS #ImageJ #Jargon API's 

The aim of this project is to develop an ImageJ plugin so that user( an iRODS client ) can upload / download datasets from iRODS . And it also provide GUI for simplicity of a user

### Implementation abstract:

-   As an implementation part first i use the Jargon Core API’s so that we can
    Jargon-core API’s implements the iRODS protocol, and allows development of
    iRODS-enabled Java applications. This API is especially useful for developing
    mid-tier applications and services, as well as desktop-clients (such as iDROP).
    These libraries also provide a foundation for a new set of interfaces that will 
    come with iRODS
    
    For adding a GUI to the plugin, I will use AWT or Swing components like Text
    Fields , Label , Buttons etc . By using AWT APIs and Swings . We can also use
    GenericDialog class as build a plugin and plugin will bemacro - compatible
    with this or we can use it like traditional way

### Implementation abstract:

-   Firstly , there are approx. 10 libararies in Jargon API’s each one has its own
    function so firstly we use Authenticate our connection with iRODSusing
    Jargon-core library( base library for implementing the protocol ) which
    contain several methods for implementing the connction-authenticating
    methods in AuthenticationConnectionclass etc and use initialize
    connection methods in such as initializeConnection() methods in
    Connection Class

-   Then we can chaecking our connection by using Jargon Data Utils
    library in which we  can use Connection Tester Class for implementing
    the above features
    
-   Then we can use Jargon Data Utils library again for adding the functionality 
    to manage the iRODS data such as building the treeusing TreeUtilityclass methods
    
-   For any type of Account information / Profile Information we may use
    Jargon User Profile library

-   IMP part for uploading or downloading a directory from iRODS we use
    getUploadDirectory()  or deleteUploadDirectory() method in the
    JargonDataUtilslibrary
    
 -  For downloading a file from iRODS we use getFile() methods from
    Jargon Data Utils library. For rest of the API’s we required we can 
    further Refrence from the Google

-   Furthur for adding GUI to the plugin we design it like a traditional way or as
    Mentors wishes . We may use GenericDialogClassfor macro compatibl plugin

-   Later We Integrate the plugin with DropBox account plugin was previously made 

## Authors

-   **Burhanuddin Bhopalwala** - _Initial work_ - [GitHub](https://github.com/burhanuddinbhopalwala)

## Acknowledgments

-   https://irods.org/clients/
-   https://imagej.nih.gov/ij/download.html
-   https://github.com/DICE-UNC/jargon

## License

[MIT](https://choosealicense.com/licenses/mit/)
