.. _WP_FAIL2BAN_ADDON_CF7_ENABLED:

.. role:: php(code)
   :language: php

WP_FAIL2BAN_ADDON_CF7_ENABLED
-----------------------------

.. rubric:: Lock Contact Form 7 spam logging on or off.

----

Fixes whether the add-on logs Contact Form 7 spam submissions. When the
constant is defined, it overrides the saved WordPress option
``wpf2b_addon_cf7_enabled`` and locks the QuickStart card and the Contact
Form 7 settings **Enabled** control.

A :php:`true` value keeps logging on; a :php:`false` value keeps it off.
Without the constant, a missing option defaults to enabled. Disabling the
add-on stops message registration and the Contact Form 7 spam hook without
removing the settings UI that turns it back on.

.. code-block:: php
   :caption: Example: Disable Contact Form 7 spam logging

   define('WP_FAIL2BAN_ADDON_CF7_ENABLED', false);

**Accepted values:** :php:`true` or :php:`false`

**Default:** enabled (the option is absent or stores ``'1'``)

The option stores only the strings ``'0'`` and ``'1'``. Free and Premium both
save the option unless a PHP constant locks it.

.. rubric:: History
.. versionadded:: 3.0.0
