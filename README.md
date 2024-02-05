# SSIS-Lab
<h1>🚀 Excited to share some recent SSIS package designs!</h1>
1- Transferred Department data from [DB] to [other] using a wizard. Ensured a clean slate by truncating the Department table before the transfer.
2- Created another wizard-based SSIS Package to export Student data (St_id, St_Fname, St_lname, St_address) from [DB] to "txt" with column names in the first row.
3- Custom SSIS Package for Student data transfer to [DB]:
a- Cleared existing data in the Student table using [Execute SQL Task].
b- Merged first and last names into a new field [Full name] with [Derived Column Component].
c- Implemented a full backup for [DB].
d- On error, a message box displays an error message.
4- Split Course data from [DB] into 3 files:
a- Selected Course data with a specific topic from DB.
b- Sorted Course data by Crs_name in descending order using [Sort Component].
c- Converted Crs_name to lowercase with [Character Map Component].
d- Split data into three files based on Course Duration, setting column names in the first row.
5- Merged "File1.txt" and "File2.txt" into one file:
a- Utilized [Merge Component] with sorting by Crs_name.
b- Combined the files using [Union Component].
