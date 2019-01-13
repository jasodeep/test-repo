# Grievance Portal
This is a [Drupal 8](https://www.drupal.org/8) installation site powered by [Docksal](https://docksal.io).

### Stack
* apache2.4
* mysql-5.6
* php7.1
* memcached
## Setup Instructions
### Step 1: Environment setup
* Install **Docksal**. [Installtion Guide](https://docksal.io/installation).
* Install **AWS Command Line Interface**. [Installtion Guide](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)
### Step 2: Project Setup
**1.** Clone this repo into your Projects directory
```
git clone git@github.com:innoraft/grievance-portal.git grievance-portal
cd grievance-portal
```
**2.** Copy and rename the file `.docksal/example.docksal-local.env` to `.docksal/example.docksal-local.env`
```
S3_BUCKET=
S3_PREFIX=
AWS_ACCESS_KEY_ID=
AWS_SECRECT_ACCESS_KEY=
```
**2.** Copy and rename the following files
`.config/default/default.settings.php` to `.docksal/settings.php` 
and 
`.config/default/default.settings.local.php` to `.docksal/settings.local.php` 
