# Grievance Portal
This is a [Drupal 8](https://www.drupal.org/8) site powered by [Docksal](https://docksal.io).

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
**1.** Clone this repo into your projects directory
```
git clone git@github.com:innoraft/grievance-portal.git grievance-portal
cd grievance-portal
```
**2.** Copy and rename the file `.docksal/example.docksal-local.env` to `.docksal/docksal-local.env`
```
S3_BUCKET=
S3_PREFIX=
AWS_ACCESS_KEY_ID=
AWS_SECRECT_ACCESS_KEY=
```
**2.** Copy and rename the following files <br>
`.config/default/default.settings.php` to `.docksal/default/settings.php` <br>
`.config/default/default.settings.local.php` to `.docksal/default/settings.local.php` 
<br><br>
**3.** Enter database credentials in `.docksal/settings.local.php` 
```
$databases['default']['default'] = array (
  'database' => '',
  'username' => '',
  'password' => '',
  'host' => '',
  'driver' => '',
);
```
**4.** Install the site. <br>
Run the following command in the project root
```
fin init
```

**5.** Open the URL in the browser.
```
http://grievanceportal.local
```

## Notes

```
# start project
fin up

# check logs
fin log
```
