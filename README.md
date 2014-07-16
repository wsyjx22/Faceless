# Faceless

Faceless is where you can talk freely. Share messages with your friends and the whole world.

## Demo

[Get the free Android app from Google Play](http://www.delight.im/get/faceless)

## Installation

### Server

 1. Set up a web server with Apache + PHP + MySQL
 2. Set up a Twilio account and register an SMS-enabled phone number POSTing to the public URL of `Server/htdocs/internal/sms_verify.php`
 3. Rename `Server/config.example.php` to `Server/config.php` and replace all occurrences of `REPLACE_THIS_WITH_VALUE` with a proper configuration value for your setup
 4. Set up cron jobs for `htdocs/workers/dispatcher.php`, `htdocs/workers/score_updater.php` and `htdocs/workers/cleaner.php`

### Android

 1. Rename `Android/src/im/delight/faceless/ConfigExample.java` to `Android/src/im/delight/faceless/Config.java` and replace all occurrences of `REPLACE_THIS_WITH_VALUE` with a proper configuration value for your setup
 2. Import all [dependencies](Android/README.md#dependencies) for the Android project

## Security

[Disclose bugs and vulnerabilities](http://www.delight.im/security/faceless) or read more about [security](SECURITY.md).

## Translations

[Faceless on Localize](http://www.localize.io/v/36)

## Known issues

### Android

 * The app cannot be installed on devices without telephony features (e.g. tablets). This is because (a) the app is optimized for phones and (b) users would have to enter their phone number manually, otherwise, and (c) the app curently can run on a single device only.

## Similar services

 * [Secret](http://www.secret.ly/)
 * [Whisper](http://whisper.sh/)
 * [Yik Yak](http://yikyakapp.com/)
 * [Experience Project](http://www.experienceproject.com/)
 * [PostSecret](http://postsecret.com/)

## License

```
Copyright (C) 2014 www.delight.im <info@delight.im>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see {http://www.gnu.org/licenses/}.
```