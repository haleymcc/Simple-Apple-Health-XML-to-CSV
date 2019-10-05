# Simple Apple Health XML to CSV

A simple script to convert Apple Health's export.xml file to an easy to use csv.



## How to Run

1. ####Verify you have pandas installed on your machine or environment

`python -c "import pandas"` should return blank from the command line

If you get a _**ModuleNotFoundError: No module named 'pandas'**_ error, install pandas:

`pip install pandas`



2. ####Export your Apple Health Data

   Go to your health home screen and click on the profile icon

<img style="float: left;" src="health_home.PNG" width=300>

On the next page, click the "Export Health Data" button

<img style="float: left;" src="export_data_button.jpg" width = 300 >

Your data will be prepared, and then you can transfer the export.zip file to your machine.

3. Unzip the file, which should contain:

   * apple_health_export
     * export.xml
     * export_cda.xml

4. Place the **apple_health_xml_convert.py** into the folder alongside the files

5. Run the script with `python apple_health_xml_convert.py`

   

The export will be written with the format:

* **apple_health_export_YYYY-MM-DD.csv**

