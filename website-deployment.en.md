[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Website deployment made easy with Rocketeer
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## Grav CMS Pro website deployment strategy

  **Website deployment** is a serious task. In fact, when you use the wrong strategy, you might go into troubles and have your website completely broke down for a long time.

  There are many ways to deploy a website, the best one in our opinion is using git. By default our all projects are managed through git, so leveraging it for deploying our websites was a natural step.
  ==|

  Now we will explain our deploying strategy so you can understand if it could fit well for you too.

  ### How we can use git for deploying a website

  Using git for deploying a website requires a remote repository, you can get one for free on Github or Bitbucket. Next, the server where your website lives must be able to pull from the GIT remote repository in order to get the changes you have committed.

  In detail, you work on your website on your laptop and you push your changes to your remote git repository. When you are done, you go to your remote server and then you pull the changes from the remote repository and your site is immediately updated.

  Working this way, your previous website version remains the active one until the pulling process has completed. When the operation is done, the new website version takes place transparently without any break or downtime.

  ### Automate the deploy process

  Maybe, you would wonder if you must log in into your remote server and manually run a pull from a git repository, this additional step can be automate with a script.

  The easy way to automate the process is adding a script which is activated by a hook from a remote git repository. The hook event is raised every time the repository gets a push. This approach works fine but every time you push, your website is updated and this is something you do not always want.

  Here is where [Rocketeer](http://rocketeer.autopergamene.eu/) comes into play.

  ### Rocketeer

  ![Website deployment with Rocketeer](/user/pages/images/website-deployment.gif "Website deployment"){.responsive-img}

  Rocketeer is a php console application which takes care to deploy websites using git. It has several awesome features to cover all the deployment aspects, the most important are:

  - [m-icon icon="fa-check"][/m-icon] Deploy websites
  - [m-icon icon="fa-check"][/m-icon] Update websites
  - [m-icon icon="fa-check"][/m-icon] Rollback to previous or specific version
  - [m-icon icon="fa-check"][/m-icon] Multi enviroments
  - [m-icon icon="fa-check"][/m-icon] Additional task

  **Deploy** and **update** commands do the same thing and the difference is that a deploy creates a new release, while update doesn't, because it updates the current version.

  **Rollback** is an awesome feature that let you go back to previous or to a specific version in seconds when something goes wrong. When bad things happens, is better to be safe than sorry!

  You can define as many **environments** as needed, so you can have a stage environment configured on a subdomain of your website you can deploy to check if everything is fine, before deploying to the production environment.

  ### Website caching

  Speed is essential to avoid a user leaves your website before it opens and Grav is very fast most of the times, but on a shared hosting, it could be dramatically slow. The problem can be overcome using the  **Advanced pagecache plugin**.

  This plugin basically caches every page when it is opened the first time so the second time it loads that page from cache bypassing all grav processes. Using that plugin, your website becomes as fast as a native html site.

  This means the whole website must be parsed the first time to have it cached properly. The **Material plugin** comes with a built-in command launched by  **Rocketeer at the end of the deployment process** which make sure all the pages in your website are open and cached successfully.

  ![Website caching during Rocketeer deployment](/user/pages/images/website-caching.gif "Website caching"){.responsive-img}

  As you can see in the screenshot above, Rocketeer parsed the whole **gravcmspro.com** website at the end of the deployment.

  ### What you get

  While configuring Rocketeer is pretty simple, we will give you a completed configuration you just need to configure to reflect your parameters.

  In detail you get:

  - [m-icon icon="fa-check"][/m-icon] Rocketeer full configuration
  - [m-icon icon="fa-check"][/m-icon] Stage and production environments
  - [m-icon icon="fa-check"][/m-icon] Additional task already configured
  - [m-icon icon="fa-check"][/m-icon] Detailed instruction about configuring Rocketeer parameters, Bitbucket account and SSH protocol on your remote server.

[/m-dictionary-item]
