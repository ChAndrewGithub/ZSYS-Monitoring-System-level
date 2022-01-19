Instructions:

Developed in: Visual Studio 2012 Ent + Final Patch MVC 5 

Tested: 
Microsoft Windows 2016 Standard English 64bit
Microsoft SQL Server Express 2019
SQL Management Studio 18 English

Installation steps:
0)Set correct date and time on local server
1)install Microsoft Windows 2016 Standard English 64bit
2)Login as a local administrator to install the specified software packages
3)Install Microsoft SQL Server Express 2019, instance name SQLEXPRESS
4)Install SQL Management Studio 18 English
5)login for the first time to change password in z/os


Unpack archive and copy to C:\
Run the installer C:\Addon_IBM_zSystems_v1\Install\Addon_for_IBM_PM.exe and follow the instructions.


After install:
http://hostname:8806 – web resource for working with the service for collecting data from the HMC.
http://hostname:8807 – web resource for working with the service for collecting data from the Z/OS. 
http://hostname:8808 – web resource for working with the service for collecting data from the TSM.
http://hostname:8809 – web resource for multi-user work with the received data

User Access: Allowed to login for users added to the “Administrators” group:
      C:\Addon_IBM_zSystems_v1\Addon_IBM_zSystems_v1_WA_DataCollectionZSYS_after_pub\Web.config ->
                                                                    <system.web>
                                                                    <authorization>
                                                                     <allow roles="Administrators"/>
                                                                    </authorization>
                                                                    </system.web>
      C:\Addon_IBM_zSystems_v1\Addon_IBM_zSystems_v1_WA_DataCollectionHMC_after_pub\Web.config ->
                                                                    <system.web>
                                                                    <authorization>
                                                                     <allow roles="Administrators"/>
                                                                    </authorization>
                                                                    </system.web>
      C:\Addon_IBM_zSystems_v1\Addon_IBM_zSystems_v1_WA_DataCollectionTSM_after_pub\Web.config ->
                                                                    <system.web>
                                                                    <authorization>
                                                                     <allow roles="Administrators"/>
                                                                    </authorization>
                                                                    </system.web>
      C:\Addon_IBM_zSystems_v1\Addon_IBM_zSystems_v1_WA_Reporting_after_pub\Web.config ->
                                                                    <system.web>
                                                                    <authorization>
                                                                     <allow roles="Administrators"/>
                                                                    </authorization>
                                                                    </system.web>
 
