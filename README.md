# ORACLE_PDB_Assigment2_30653-2025-mohamed



Oracle Pluggable Database (PDB) Administration
1. Assignment Overview
The objective of this assignment is to develop practical Oracle Database Administration skills by implementing Oracle Multitenant Architecture, specifically focusing on creating, managing, and deleting Pluggable Databases (PDBs), as well as configuring database users and documenting the entire process.
2. Oracle Environment
 Oracle Version: Oracle AI Database 23ai Free Release 23.26.1.0.0
 Operating System: Kali Linux (Docker Container)
 Tools Used: * Docker
 SQL*Plus
 Firefox (for OEM attempts)
3. Task Documentation
Task 1: PDB Creation and User Configuration
 PDB Creation: Successfully created the PDB named ⁠mo_pdb_306532025⁠ using the ⁠FILE_NAME_CONVERT⁠ parameter from the seed database.
 User Creation: Created the user ⁠mohamed_plsqlauca_306532025⁠ inside the PDB and assigned the necessary ⁠DBA⁠, ⁠CONNECT⁠, and ⁠RESOURCE⁠ privileges.
 Verification: Successfully logged into the PDB using the new user credentials.
Task 2: Temporary PDB Creation and Deletion
 Creation: Created a temporary PDB named ⁠mo_to_delete_pdb_306532025⁠ for testing purposes.
 Deletion: Verified the existence of the PDB, then successfully closed and dropped it, including all associated datafiles, to ensure a clean environment.
Task 3: Oracle Enterprise Manager (OEM) Configuration
 Attempted to configure and access the OEM dashboard via port 5500.
4. Challenges and Solutions
 Challenge: I was unable to access the Oracle Enterprise Manager (OEM) dashboard via the browser at ⁠https://localhost:5500/em⁠ despite attempting to enable the HTTPS port using ⁠EXEC DBMS_XDB_CONFIG.SETHTTPSPORT(5500);⁠ within the SQL*Plus environment. The browser consistently displayed an "Unable to connect" error.
 Troubleshooting Steps Taken:
1. Verified that the Oracle container was running with the correct port mapping.
2. Attempted to manually set the HTTPS port using SQL*Plus.
3. Tried different browser configurations and protocols.
 Resolution: Due to the limitations of the Oracle 23ai Free Docker environment, the full OEM Express service was not accessible. As a workaround, I have demonstrated the environment details, PDB status, and instance configuration using the SQL*Plus command-line interface, which confirms the successful setup and management of the database.
5. Lessons Learned
By completing this assignment, I gained hands-on experience in:
 Managing Oracle Multitenant architecture.
 Handling container-based database environments.
 Troubleshooting connectivity issues in Dockerized Oracle instances.
 Professional documentation and repository management on GitHub.
6. Integrity Statement
"I confirm that this assignment represents my own practical work, screenshots, and documentation. All external resources consulted have been properly acknowledged."
