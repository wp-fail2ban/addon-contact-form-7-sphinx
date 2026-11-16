.. _release:

===================
Release information
===================

WP fail2ban Contact Form 7 3.0.0
--------------------------------

Version 3.0.0 updates the add-on for the supported WP fail2ban 5.x and 6.x
interfaces and adds an operator-facing enable switch for Contact Form 7 spam
logging.

Reader-visible changes in this release include:

* QuickStart and the Contact Form 7 settings **Enabled** control turn spam
  logging on or off (default enabled);
* :ref:`WP_FAIL2BAN_ADDON_CF7_ENABLED` locks that choice from
  ``wp-config.php``;
* with logging off, the add-on registers no messages and does not hook Contact
  Form 7, while the settings UI remains available.
