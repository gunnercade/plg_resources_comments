# plg_resources_comments
Makes a Comments tab in Resources Component in a HUBzero CMS version 2.2

The Comments tab allows registered users to post a Comment, either under their own name or anonymously, for a Resource in a HUBzero CMS Resource. The owner of the Resource receives an email notifying them that someone has commented on their resource. The purpose of this tab is to facilitate discussion of a Resource or allow a user to correspond with the author about that particular resource.

This Comments tab plugin was developed by Shawn Rice at HUBzero and is subject to the copyright notice therein.

INSTALLATION DIRECTIONS:

1) Unzip this file. Then you'll need to move things to the appropriate place in your HUB's installation: 

a) You'll need to place the Migrations file at WEBROOT/app/migrations/Migration20160930122701PlgResourcesComments.php

b) Place the remaining files at WEBROOT/app/plugins/resources/comments/

2) Now run migrations:
'/var/www/SITENAME/$ php muse migration -f'

3) Log into the backend as an admin and look at Component > Resources and go to the Plugins tab. You should see a Plugin named "Resources-Comments."

4) To turn on the Comments tab for a specific Resource type, go to Component > Resources and look at the Types tab. Click the name of the Resource type you would like to have the Comments tab. Now look for the Plugin "Resources-Comments" in the list on the right hand side and click the radio button to turn it "on."

You should now be able to go to the frontend of your website, browse to a Resource of the appropriate type from step (4) and see the Comments tab. If you are logged in, you should be able to post a comment.
