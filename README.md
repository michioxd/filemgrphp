<h3 align="center">
    <img alt="Logo" src="https://i.imgur.com/cDcnWac.png" width="200"/>
</h3>

<h1 align="center">
  FileMgrPHP
</h1>
<p align="center">
    FileMgrPHP - PHP-based Multi-function File Manager
</p>
<p align="center">
    <a href="https://www.gnu.org/licenses/gpl-3.0"><img alt="License GPLv3" src="https://img.shields.io/badge/License-GPL_v3-blue.svg"></a>
    <a href="https://jquery.org"><img src="https://img.shields.io/badge/jquery-%230769AD.svg?style=for-the-badge&logo=jquery&logoColor=white" alt="jQuery"></a>
  <a href="https://php.net"><img src="https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white" alt="PHP"></a>
</p>

![](https://i.imgur.com/iEIJjec.png)

# Features
- Multi-language support
- Multi-file select (Selection Rectangle is support ([Selection by Simonwep](https://github.com/Simonwep/selection)))
- Multi-file upload
- Delete/Move/Copy
- Material Design UI ([MDUI](https://github.com/zdhxiong/mdui))
- File editor ([Ace Editor](https://github.com/ajaxorg/ace))
- Multimedia player/streaming (Video/Image/Music)
- Zip Archive Un/compresss
- Dark mode support
- Ribbon navigator support

# Language
Currently we support the following language:
- English
- Vietnamese (Tiếng Việt)

You can help me translate FileMgrPHP to support more language. [Check this](TRANSLATION.md)

# Installation
Download filemgr.php, upload it to your server, open it with your favorite code editor (Notepad is okay). You will see the configuration array start from line 14
```php
$config = array(
    // Document root, use $_SERVER['DOCUMENT_ROOT'] if you don't know what this is
    'document_root' => $_SERVER['DOCUMENT_ROOT'], 

    // Never use password, recommended to keep this false
    'never_use_password' => true, 

    // Password to access the file manager (use genPass.php to generate a password) (default: admin@123)
    'password' => 'JDJ5JDEwJENEQW5LS1dudlNaWDJQQy9Kdnc0dWVOeDNCdzdYV0VQTzQzRWZETTZoR2RDN0lQLjRRMDdL', 

    // Session type, this will using cookie or PHP Session to save your session (session()) (option: 'cookie' or 'session', default: cookie)
    'session_type' => 'cookie', 

    // Session expire, this will set your cookie expire time (skip it if you use session mode) (default: 86400 (24 hours))
    'session_expire' => '86400',

    // Default language, this will set your default language (default: 1 = English). 0 = English, 1 = Tiếng Việt (Vietnamese)
    'default_language' => 0,

    // Read only mode, this will set your file manager to read only mode (default: false)
    'read_only' => false, 

    // Use it if you don't want to download the FileMgrPHP resouces, you need only one file (filemgr.php) to run (default: true)
    'online_cdn' => true 
);
```
