# CiviCRM Pantheon/Lando Settings 

While hacking this config file together for a new project, I noticed there wasn't much information out there about integrating CiviCRM with a WordPress site hosted on the Pantheon platform, so I thought I'd share what I came up with. These settings are specifically designed to use the $_SERVER environment variable made available by Pantheon servers as well as the Lando development environment. This allows you to develop and maintain your WordPress/CiviCRM site in peace without worrying about any snags when moving the code & database between environments. I'm new to CiviCRM so I'm sure this code could use some improvement, if you find it helpful please contribute! In particular, it would be great to to find some info on improving the performance of Smarty on Pantheon, or any settings to integrate with Redis.

### Prerequisites

* [Pantheon](https://dashboard.pantheon.io/register) - Container based hosting platform for WordPress and Drupal sites
* [Lando](https://github.com/lando/lando) - Open source, cross-platform, local development environment and DevOps tool built on Docker
* [CiviCRM](https://civicrm.org/download) - Open source contact relationship management system

### Installing

After you've got a WordPress site up and running and installed CiviCRM, place the settings file in 

```
wp-content/uploads/civicrm/
```

The settings file will then allow you to sync your database between your local dev environment and the development, testing, and live servers without worrying about any nasty errors or manually editing any credentials.

## Authors

* **Paolo Matchett** - *Initial work* - [Front Group Design](https://frontgroupdesign.com)

## Acknowledgments

* Some code taken and modified from this very helpful [Kalamuna blog post](https://blog.kalamuna.com/news/civicrm-pantheon)

