# Wodpress Site Restoration
This Repo had pre-installed set of plugins to be able to restore web site backed up using ```updraftplus(version 1.16.49)``` plugin

----
## How to restores

- bring up container with <br>
 ```docker-compose up -d```
- apply wp-config.patch <br>
    ```cd wordpress/ && git apply ../wp-config.patch && cd..```
- brows to http://localhost:8080/ setup the wordpress site
- install activate updraftplus backup and Better Search and replace plugins ( ensure they are active too)
- brows to settings-->updraftplus and restore using local backed up file
- Refresh browser and this time you will need to login to wp-admin using credentials of restored site
- brows to tools-->Better Search and replace , replace original sitename with http://localhost

----
## Notes
 - This setup is locked to wordpress version 5.2.6 and php 7.3
 - site restroe was tested using version 1.16.49 of updraftplus
 - site name was replacement was tested using verion 1.3.4 of Better Search and Replace

 **newer version of plugins should work but,it is not guaranteed**
 