.. _WP_FAIL2BAN_ADDON_CF7_ENABLED:

.. role:: php(code)
   :language: php

WP_FAIL2BAN_ADDON_CF7_ENABLED
-----------------------------

.. rubric:: Lock Contact Form 7 spam logging on or off.

----

Fixes whether the add-on logs Contact Form 7 spam submissions. When the
constant is defined, it locks the QuickStart card and the Contact Form 7
settings **Enabled** control to that value.

A :php:`true` value keeps logging on; a :php:`false` value keeps it off.
Without the constant, logging defaults to enabled and operators can change it
from QuickStart or the Contact Form 7 settings tab. Disabling the add-on stops
message registration and the Contact Form 7 spam hook without removing the
settings UI that turns it back on.

.. code-block:: php
   :caption: Example: Disable Contact Form 7 spam logging

   define('WP_FAIL2BAN_ADDON_CF7_ENABLED', false);

**Accepted values:** :php:`true` or :php:`false`

**Default:** enabled

Free and Premium both honour the UI controls unless a PHP constant locks them.

.. rubric:: History
.. versionadded:: 3.0.0
