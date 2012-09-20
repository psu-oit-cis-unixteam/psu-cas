Portland State University CAS
=============================

Our Maven build for our local CAS overlay.

This build process presently emits a WAR and RPM.

To build for production:
------------------------
    mvn clean package

To build without jBoss (for single node testing):
-------------------------------------------------
    mvn clean package -Pdevelopment

To change built version and dependency versions:
-------------------------
- Refer to the \<properties\> block of pom.xml, it contains the locally
  maintained package version number and also selects versions of CAS, etc.
