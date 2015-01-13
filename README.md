## Password change plugin for WebMail Lite @ AfterLogic

#### 1. Put the plugin file in 'data/plugins/postfix-dovecot-password/index.php'
Download or copy index.php from my Git repo and put it in your destination path.

#### 2. Run plugin and configure it.
Then, you should run plugin in: data/settings/config.php (append to array):
```
'plugins.postfix-dovecot-password' => true,
```

Next to set correctly database settings with your postfix configuration tables:
```
'plugins.postfix-dovecot-password.config.host'       => '127.0.0.1',
'plugins.postfix-dovecot-password.config.dbuser'     => 'your-db-user',
'plugins.postfix-dovecot-password.config.dbpassword' => 'your-db-password',
'plugins.postfix-dovecot-password.config.dbname'     => 'your-db-name',
```
Optional you can overwrite column names settings:
```
'plugins.postfix-dovecot-password.config.mailbox_table'   => 'mailbox',
'plugins.postfix-dovecot-password.config.username_column' => 'username',
'plugins.postfix-dovecot-password.config.password_column' => 'password',
```

#### 3. Enjoy.
