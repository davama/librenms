source: Extensions/Webssh2.md
path: blob/master/doc/

# Webssh2 integration

We have simple integration for
[Webssh2](https://github.com/billchurch/webssh2), you will be redirected
to your Webssh2 command line frontend to access your
equipment. (Currently this only works with SSH)

Webssh2 itself isn't included within LibreNMS, you will need to
install this separately either on the same infrastructure as LibreNMS
or as a totally  standalone appliance. The installation is beyond the
scope of this document.

Config is simple, include the following in your `config.php`:

```php
$config['webssh2']['server'] = 'http://<your_webssh2_url/';
```

**Note:** You *must* use the full url including the trailing `/`!

**Tip:** Having SSO configured on your infrastructure will make your webssh2 authentication more seamless.
