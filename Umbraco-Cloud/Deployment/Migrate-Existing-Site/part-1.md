# Prepare your site for migration

After making sure that your project(s) meets all the [requirements](index.md) for being migrated to Umbraco Cloud, you are now ready to get started!

## Upgrade to latest Umbraco version
First order of business is to upgrade your own project to the latest Umbraco version. Why? Because Umbraco Cloud always runs the latest version and you need to make sure your project runs the same Umbraco version as Umbraco Cloud.
You can download the latest version of Umbraco from [Our](https://our.umbraco.org/download/).
If you need help upgrading your project, we have some excellent [Upgrade instructions](https://our.umbraco.org/documentation/Getting-Started/Setup/Upgrading/general) you can follow. Be thorough when upgrading, as the latest upgrade might contain breaking changes and/or updated configuration.

After upgrading your project make sure it runs without any errors. *Hint: Check the umbracoTraceLog.txt log file.*  
Ideally your site will run locally using the SQL CE database as this will make content migration easier. Don't worry - if that's not possible you will still be able to complete the migration.

## Cleaning your project
Now you're almost ready to start the actual migrating! The only thing left to is to clean up the your project a bit.

While the project is still running you need to:

  * Go the backoffice of your project
  * Empty the Content and Media Recycle bins

Shut down the project, and delete the following files and folders from `/App_Data`

  * `/TEMP`
  * `/Logs`
  * `/cache`
  * `/preview`
  * `umbraco.config`

![delete-from-app-data](images/App_Data-DELETE.png)

That was it! Now you are ready to start the actual migraion process, or in other words: **now the real fun begins!**

[Up next: Merge with your Cloud project](part-2.md)
