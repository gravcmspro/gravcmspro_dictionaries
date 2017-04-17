[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Website deployment made easy with Rocketeer
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## Grav CMS Pro website deployment strategy

  **Website deployment** is a serius task. In fact, when you use a wrong strategy, you might went in troubles and have your website broke down for a long time.

  There are many ways to deploy a website, the best one in our opinion is using git. By default our all projects are managed through git, so leveraging it for deploying our websites was a natural step.
  ==|
  
  Now we will explain our deploying strategy so you can understand if it could fit well for you too.

  ### How we can use git for deploying a website

  Using git for deploying a website requires a remote repository, you can get for free at Github or Bitbucket. Next, the server where your website lives, must be able to pull from the remote repository to get the changes you commited.

  In detail, you work on your website on your laptop and you push your changes to your remote git repository. When you are done, you go to your remote server and then you pull the changes from the remote repository and your site is immediately updated.

  Working this way, your previous version remains the active one until the pulling is completed and when this operation is finished at last, the new website version take place without any break.

  ### Automatize the deploy process

  Maybe you would wonder if you must enter into your remote server and manually run a pull from git repository. Obviously you don'o't.

  The easy way to automatize that process is adding a script which is activated by an hook from remote git repository. The hook event is raised every time the repository gets a push. This approach works fine but everytime you push, your website is updated and this is something you do not always want.

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

  **Rollback** is an awesome feature that let you go back to previous or to a specific version in seconds, when something goes wrong. And, belive me, bad things happen!

  You can define as many **enviroments** you need, so you can have a stage environment configured on a subdomain of your website you can deploy to check if everything is fine, before deploy to production enviroinment.

  ### Website caching

  Speed is essential to avoid a user leaves your website before it opens and Grav is very fast the most of times, but, on shared hosting, it could be drammatically slow. That problem can be overcome using the **Advanced pagecache plugin**.

  This plugin basically caches every page when it is opened the first time so the second time it loads that page from cache bypassing all grav processes. Using that plugin, your website becomes as fast as a native html site.

  This means the whole website must be parsed the first time to have it cached properly. **Material plugin** comes with a built-in command launched by **Rocketeer at the end of deployment** which takes care to open all the pages of your website to have them cached as well.

  ![Website caching during Rocketeer deployment](/user/pages/images/website-caching.gif "Website caching"){.responsive-img}

  As you can seen in the screenshot above, Rocketeer parsed the whole **gravcmspro.com** website at the end of the deployment.

  ### What you get

  While configuring Rocketeer is pretty simple, we will give you a completed configuration you just need to configure to reflect your parameters.

  In detail you get:

  - [m-icon icon="fa-check"][/m-icon] Rocketeer full configuration
  - [m-icon icon="fa-check"][/m-icon] Stage and production environments
  - [m-icon icon="fa-check"][/m-icon] Additional task already configured
  - [m-icon icon="fa-check"][/m-icon] Detailed instruction about configuring Rocketeer parameters, Bitbucket account and SSH protocol on your remote server.

[/m-dictionary-item]
