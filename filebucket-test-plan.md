# Filebucket Dev Test Environment

1. FileBucket Requirements
    1. All the nodes stood up - complete
    1. Configuration for minIO - complete 
    1. Needs a reverse proxy setup - complete
        1. still need to config nginx for reverse proxy - 
    1. Another bucket for dummy test bucket
        1. Replicate Eric's data in to a test buckets
        2. Eric to provide the path
3. Environment Side
    1. Claim an environment and configure
    1. Using the test database 
    1. Use Dev filebucket data. 
    1. Reference with an nfs mount (now).  
    1. UNC path to the files. 
    1. Dev 
        1. admin 
        1. customer 
        1. imaging - currently working on. blocked by S3 fuse.
        1. microservices
            1. Depending on the mount point - the core machine would pass through via UNC pathing. 
            2. for kiss cut 
        3. PHP API
            1. separate instance for gearman
            2. windows mount will look like samba
        3. upload server doesn't exist for dev
# TouchPoint Meeting 3/29/22

1. Outstanding Tasks
    2. Issue with minIO - Resolved and corrected.
    3. REHL Upload Server being worked on by Karim - 
        1. Resolved
        1. Paste commands for Eric/Karim to reregister with the entitlement server.
    1. nginx not available - recognized reverse proxy - Resolved.
    1. PHP -  
    1. New REHL License booted us off the Entitlement server - Today - should be resolved.
    1. Setup S3 Fuse - currently working on it.
        1. Once we know we can read/write to the locations.
            1. We can begin testing end to end.
            1. 
            1. 

|Task|Assigned to |Status|Notes|
|---|---|---|---|
|Issues with MinIO|Jonathan|Resolved| |
|RHEL Upload Server|Karim| Resolved| |
|Imaging Server| Karim|Open||
|PHP setup| Eric|Resolved||
|New RHEL License - Entitle Server|Jonathan|Resolved||
|S3 Fuse install and configuration|Jonathan|Open|Installed, performance tuning for file access. working on serving files.  Still trying to get into reading rsync data.


1. Plan on to cut over images
    1. Can't cut over in a split fashion
    1. once we figure out rsync - reading correctly by minIO
        1. plan on rsync
    2. Object storage doesn't have directory structure.




