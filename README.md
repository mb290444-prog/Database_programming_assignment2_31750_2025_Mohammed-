# Database Programming Assignment

## Task 1: Creating and Opening a Pluggable Database (PDB)

I successfully created the Pluggable Database `MO_PDB_31750_2025` and opened it in `READ WRITE` mode.

### Commands Used:
CREATE PLUGGABLE DATABASE MO_PDB_31750_2025 ADMIN USER mohammed_31750 IDENTIFIED BY 123456 FILE_NAME_CONVERT=('pdbseed', 'MO_PDB_31750_2025');
ALTER PLUGGABLE DATABASE MO_PDB_31750_2025 OPEN;
SHOW PDBS;
<img width="853" height="387" alt="task1_pdbb_created_and_opened" src="https://github.com/user-attachments/assets/9fc438ff-8961-4b5f-9563-c1aacbc7cbc4" />
# Database Programming Assignment

## Task 1: Creating and Opening a Pluggable Database (PDB)

I successfully created the Pluggable Database `MO_PDB_31750_2025` and opened it in `READ WRITE` mode.

### Commands Used:
CREATE PLUGGABLE DATABASE MO_PDB_31750_2025 ADMIN USER mohammed_31750 IDENTIFIED BY 123456 FILE_NAME_CONVERT=('pdbseed', 'MO_PDB_31750_2025');
ALTER PLUGGABLE DATABASE MO_PDB_31750_2025 OPEN;
SHOW PDBS;



## Task 2: Create and Delete a Temporary PDB

I have successfully created a temporary PDB, opened it, and then completely removed it including its datafiles.

### Commands Used:
CREATE PLUGGABLE DATABASE MO_TO_DELETE_PDB_31750 ADMIN USER admin_temp IDENTIFIED BY 123456 FILE_NAME_CONVERT=('pdbseed', 'MO_TO_DELETE_PDB_31750');
ALTER PLUGGABLE DATABASE MO_TO_DELETE_PDB_31750 OPEN;
ALTER PLUGGABLE DATABASE MO_TO_DELETE_PDB_31750 CLOSE;
DROP PLUGGABLE DATABASE MO_TO_DELETE_PDB_31750 INCLUDING DATAFILES;
SHOW PDBS;

<img width="937" height="482" alt="task2_pdb_created_and_deleted" src="https://github.com/user-attachments/assets/1e296f2e-c5b8-4bce-81cd-3280cfea99e9" />
