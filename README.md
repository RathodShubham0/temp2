 Description:
Though mandatory text field of 'Full-load current' (in Set system inputs dialog box) is empty and user clicks on 'Save and recalculate' button, operation proceeds.

Steps to Reproduce:
Upload the document (PR) for parsing and data extraction.
Come to APS section.
Set the inputs in 'Set system inputs dialog box for System type and Full-load current.
Click on Save and recalculate button.
Now again open 'Set system inputs' dialog box.
Erase the value in 'Full-load current' text field.
Now again click on 'Save and recalculate' button.
Verify that it saves the data without fulfilment of 'Full-load current' mandatory field as well as the 'asterisks' (red stars) disappears.



Description:
Though the workflow got completed and came on last stage of Release Document and user completes that operation by Generating BOM, still UI is showing that stage into buffering.

Steps to Reproduce:
Open NX.
Open Powerbox plugin.
Complete the workflow from PR Parsing and Data Extraction to Release Document
When user goes into the Release Document stage, Generate the BOM.
Come back to workflow list.
Verify that Release Document stage is still in buffering mode.
(please refer an image)


Description:
User is able to add huge count of numerical values in the 'Full-load current' text field of Set system inputs dialog box of APD section. This creates huge number of load and count in the 'View previous value(s)' section of dialog box.
(please refer an images)
