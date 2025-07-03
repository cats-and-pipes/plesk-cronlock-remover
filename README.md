# Description

This is a simple&stupid extension to remove the ```root.crontab.lock``` file from plesk installations. \
If your provider allows you to upload extensions, you can use this extension to enable root access.

You need the privilege to upload extensions or to use the panel.ini editor.

# Howto build the extension

Create a zip file

    zip -r -9 cronlock-remover-1.0-2.zip htdocs plib meta.xml

and upload this to your plesk installation (Extensions → My Extensions → Upload Extension)

# What does it do?

Look in plib/views/scripts/index/index.phtml

It is very simple code!

# I cannot upload extensions

Try to install [panel.ini Editor](https://www.plesk.com/extensions/panel-ini-editor/) and set

    [ext-catalog]
    extensionUpload = true

Otherwise, you're out of luck.
