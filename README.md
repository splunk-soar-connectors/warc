[comment]: # "Auto-generated SOAR connector documentation"
# WARC

Publisher: Splunk Community  
Connector Version: 1\.0\.1  
Product Vendor: Generic  
Product Name: WARC  
Product Version Supported (regex): "\.\*"  
Minimum Product Version: 4\.10\.0\.40961  

This app supports the creation of WARC \(Web Archive\) for any webpage

### Supported Actions  
[test connectivity](#action-test-connectivity) - Validate the asset configuration for connectivity using supplied configuration  
[get url](#action-get-url) - Retrieve a WARC archive for the specified URL and add it to the vault  

## action: 'test connectivity'
Validate the asset configuration for connectivity using supplied configuration

Type: **test**  
Read only: **True**

#### Action Parameters
No parameters are required for this action

#### Action Output
No Output  

## action: 'get url'
Retrieve a WARC archive for the specified URL and add it to the vault

Type: **investigate**  
Read only: **True**

#### Action Parameters
PARAMETER | REQUIRED | DESCRIPTION | TYPE | CONTAINS
--------- | -------- | ----------- | ---- | --------
**url** |  required  | URL to retrieve the WARC for | string |  `url` 

#### Action Output
DATA PATH | TYPE | CONTAINS
--------- | ---- | --------
action\_result\.parameter\.url | string |  `url` 
action\_result\.data | string | 
action\_result\.data\.\*\.hash | string | 
action\_result\.data\.\*\.vault\_id | string | 
action\_result\.data\.\*\.size | numeric | 
action\_result\.status | string | 
action\_result\.message | string | 
action\_result\.summary | string | 
summary\.total\_objects | numeric | 
summary\.total\_objects\_successful | numeric | 