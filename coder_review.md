# Code Report

```
Drupal SQL Standards, Drupal Security Checks

update.php:
 +66: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +83: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +274: [critical] Use the Form API to build forms to help prevent against CSRF attacks.

includes/database/sqlite/schema.inc:
 +25: [critical] table names should be enclosed in {curly_brackets}
 +677: [critical] table names should be enclosed in {curly_brackets}

includes/database/pgsql/install.inc:
 +156: [critical] table names should be enclosed in {curly_brackets}

includes/database/pgsql/schema.inc:
 +54: [critical] table names should be enclosed in {curly_brackets}
 +99: [critical] table names should be enclosed in {curly_brackets}
 +329: [critical] table names should be enclosed in {curly_brackets}
 +420: [critical] table names should be enclosed in {curly_brackets}
 +433: [critical] table names should be enclosed in {curly_brackets}
 +611: [critical] table names should be enclosed in {curly_brackets}
 +614: [critical] table names should be enclosed in {curly_brackets}

includes/database/mysql/schema.inc:
 +489: [critical] table names should be enclosed in {curly_brackets}
 +493: [critical] table names should be enclosed in {curly_brackets}

includes/database/schema.inc:
 +318: [critical] table names should be enclosed in {curly_brackets}
 +340: [critical] table names should be enclosed in {curly_brackets}
 +363: [critical] table names should be enclosed in {curly_brackets}

includes/bootstrap.inc:
 +2823: [critical] the use of REQUEST_URI is prone to XSS exploits and does not work on IIS; use request_uri() instead
 +2826: [critical] the use of REQUEST_URI is prone to XSS exploits and does not work on IIS; use request_uri() instead

includes/common.inc:
 +7644: [critical] Potential problem: trigger_error() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

includes/errors.inc:
 +238: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

includes/form.inc:
 +1361: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +1412: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1449: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +1657: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1704: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

includes/install.core.inc:
 +958: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1180: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1181: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1327: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

includes/install.inc:
 +1236: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

includes/locale.inc:
 +954: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

modules/block/block.install:
 +321: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +344: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +367: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +393: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/aggregator/aggregator.processor.inc:
 +85: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/dblog/dblog.admin.inc:
 +326: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/field/tests/field_test.entity.inc:
 +399: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/field/tests/field_test.storage.inc:
 +290: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

modules/field/modules/options/options.module:
 +173: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

modules/field/tests/field_test.module:
 +255: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +259: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/field/tests/field_test.entity.inc:
 +399: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/field/tests/field_test.storage.inc:
 +290: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

modules/field_ui/field_ui.admin.inc:
 +376: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +382: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +831: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +1577: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1922: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/file/file.module:
 +580: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +585: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +591: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +668: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

modules/file/file.field.inc:
 +130: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

modules/filter/filter.admin.inc:
 +230: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +233: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +278: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/filter/filter.install:
 +430: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/image/image.admin.inc:
 +485: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +488: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +500: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

modules/image/image.field.inc:
 +180: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

modules/locale/locale.module:
 +304: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/locale/locale.admin.inc:
 +857: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +858: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +863: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1155: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/locale/locale.install:
 +200: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/menu/menu.admin.inc:
 +133: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +136: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +140: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/node/content_types.inc:
 +429: [critical] Potential problem: confirm_form() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/node/node.admin.inc:
 +205: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/openid/openid.module:
 +712: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/php/php.module:
 +80: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

modules/poll/poll.module:
 +397: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +405: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +417: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/profile/profile.module:
 +399: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +412: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +422: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +432: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +450: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +461: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/search/search.module:
 +989: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/simpletest/tests/batch_test.callbacks.inc:
 +98: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/simpletest/tests/error.test:
 +80: [critical] table names should be enclosed in {curly_brackets}

modules/simpletest/tests/schema.test:
 +86: [critical] table names should be enclosed in {curly_brackets}
 +87: [critical] table names should be enclosed in {curly_brackets}

modules/simpletest/simpletest.pages.inc:
 +32: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +33: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +247: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +248: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/simpletest/tests/batch_test.callbacks.inc:
 +98: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/simpletest/tests/error.test:
 +80: [critical] table names should be enclosed in {curly_brackets}

modules/simpletest/tests/schema.test:
 +86: [critical] table names should be enclosed in {curly_brackets}
 +87: [critical] table names should be enclosed in {curly_brackets}

modules/simpletest/tests/error_test.module:
 +64: [critical] table names should be enclosed in {curly_brackets}

modules/simpletest/tests/form_test.module:
 +729: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +822: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +823: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/simpletest/tests/url_alter_test.module:
 +34: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/system/system.module:
 +2888: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/system/system.install:
 +2015: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +2992: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/trigger/trigger.admin.inc:
 +152: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +187: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/update/update.manager.inc:
 +351: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +681: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +686: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/user/user.module:
 +1114: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1155: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1850: [critical] The value for the 'access callback' must always be a string which is the the name of the function - never a function call. It may also be assigned the value TRUE or FALSE if the callback is always (or never) accessible.

modules/user/user.admin.inc:
 +92: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/user/user.pages.inc:
 +101: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +107: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/backup_migrate/backup_migrate.module:
 +253: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1758: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/backup_migrate/includes/crud.inc:
 +354: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +786: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/backup_migrate/includes/filters.backup_restore.inc:
 +97: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/backup_migrate/includes/schedules.inc:
 +527: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/coder/coder_upgrade/includes/conversion.inc:
 +313: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/coder/coder_upgrade/includes/settings.inc:
 +142: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/coder/coder_upgrade/coder_upgrade.inc:
 +200: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/coder/coder_review/coder_review.module:
 +567: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +892: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +957: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/coder/coder_upgrade/includes/conversion.inc:
 +313: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/coder/coder_upgrade/includes/settings.inc:
 +142: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/coder/coder_upgrade/coder_upgrade.inc:
 +200: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/ctools/bulk_export/bulk_export.module:
 +226: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ctools/views_content/plugins/content_types/views.inc:
 +364: [critical] table names should be enclosed in {curly_brackets}

sites/all/modules/ctools/views_content/plugins/content_types/views_panes.inc:
 +420: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ctools/plugins/access/php.inc:
 +55: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/ctools/page_manager/plugins/tasks/page.admin.inc:
 +1316: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +1468: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/ctools/page_manager/page_manager.admin.inc:
 +1448: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1512: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +1669: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/ctools/includes/export.inc:
 +279: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +1132: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ctools/includes/math-expr.inc:
 +330: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/ctools/views_content/plugins/content_types/views.inc:
 +364: [critical] table names should be enclosed in {curly_brackets}

sites/all/modules/ctools/views_content/plugins/content_types/views_panes.inc:
 +420: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/devel/devel_generate/devel_generate.module:
 +345: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +361: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +515: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/devel/devel_generate/devel_generate.inc:
 +113: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/devel/devel_generate/devel_generate.inc:
 +113: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/flexslider/flexslider_example/flexslider_example.install:
 +41: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/flexslider/flexslider.admin.inc:
 +532: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/flexslider/flexslider_example/flexslider_example.install:
 +41: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/geocoder/plugins/geocoder_handler/yahoo.inc:
 +33: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/geocoder/plugins/geocoder_handler/yandex.inc:
 +33: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/geocoder/geocoder.widget.inc:
 +183: [critical] Potential problem: trigger_error() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/google_analytics/googleanalytics.admin.inc:
 +696: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +700: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/hacked/hacked.admin.inc:
 +30: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +34: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ip_geoloc/ip_geoloc_generator/ip_geoloc_generator.install:
 +12: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/jcarousel/includes/jcarousel.views.inc:
 +90: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/libraries/tests/modules/libraries_test_module/libraries_test_module.module:
 +518: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/location/contrib/location_cck/location_cck.module:
 +441: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +442: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/location/handlers/location_handler_field_location_distance.inc:
 +108: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +126: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/location/handlers/location_handler_sort_location_distance.inc:
 +96: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +114: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/location/handlers/location_views_handler_filter_proximity.inc:
 +180: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +200: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/location/location.views.inc:
 +565: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/media/file_entity/file_entity.admin.inc:
 +76: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +78: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +124: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/media/includes/media.admin.inc:
 +556: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +559: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/media/includes/MediaReadOnlyStreamWrapper.inc:
 +152: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +159: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/media/file_entity/file_entity.admin.inc:
 +76: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +78: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +124: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/menu_block/menu_block.admin.inc:
 +123: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/menu_editor/menu_editor.admin.inc:
 +136: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/panels/plugins/views/panels_views_plugin_row_fields.inc:
 +64: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/panels/plugins/task_handlers/panel_context.inc:
 +395: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/references/node_reference/node_reference.module:
 +83: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/references/user_reference/user_reference.module:
 +91: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/seckit/includes/seckit.form.inc:
 +27: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +420: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +424: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/security_review/security_review.install:
 +13: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/security_review/security_review.pages.inc:
 +31: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +331: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/simplenews/simplenews_rules/simplenews_rules.rules.inc:
 +46: [critical] table names should be enclosed in {curly_brackets}
 +92: [critical] table names should be enclosed in {curly_brackets}

sites/all/modules/simplenews/includes/simplenews.admin.inc:
 +64: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1617: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1623: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/simplenews/includes/simplenews.subscription.inc:
 +736: [critical] table names should be enclosed in {curly_brackets}

sites/all/modules/simplenews/simplenews_rules/simplenews_rules.rules.inc:
 +46: [critical] table names should be enclosed in {curly_brackets}
 +92: [critical] table names should be enclosed in {curly_brackets}

sites/all/modules/social_media_links/social_media_links.module:
 +111: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/tablefield/tablefield.module:
 +442: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +508: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/plugins/views_plugin_argument_default_php.inc:
 +53: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/views/plugins/views_plugin_argument_validate_php.inc:
 +27: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +53: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/views/plugins/views_plugin_display.inc:
 +1812: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/plugins/views_plugin_display_page.inc:
 +486: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/views/plugins/views_plugin_exposed_form.inc:
 +226: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/plugins/views_plugin_pager_full.inc:
 +59: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +61: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +399: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +411: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/plugins/views_plugin_pager_some.inc:
 +36: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +38: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/modules/user/views_plugin_argument_validate_user.inc:
 +102: [critical] In SQL strings, Use db_query() placeholders in place of variables.  This is a potential source of SQL injection attacks when the variable can come from user data.

sites/all/modules/views/modules/taxonomy/views_handler_filter_term_node_tid.inc:
 +111: [critical] table names should be enclosed in {curly_brackets}
 +111: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +193: [critical] table names should be enclosed in {curly_brackets}
 +193: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/modules/search/views_handler_filter_search.inc:
 +78: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/modules/node/views_handler_filter_history_user_timestamp.inc:
 +41: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/includes/admin.inc:
 +97: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +251: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +701: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +2005: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +2119: [critical] Potential problem: form_set_error() and form_error() only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +4122: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/includes/view.inc:
 +1937: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/views/handlers/views_handler_area_result.inc:
 +46: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/handlers/views_handler_argument.inc:
 +231: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +293: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/handlers/views_handler_filter_boolean_operator.inc:
 +105: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/handlers/views_handler_filter_in_operator.inc:
 +208: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/handlers/views_handler_filter_numeric.inc:
 +166: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +180: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +192: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +198: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/views/views.install:
 +291: [critical] In SQL strings, Use db_query() placeholders in place of variables.  This is a potential source of SQL injection attacks when the variable can come from user data.

sites/all/modules/views_slideshow/theme/views_slideshow.theme.inc:
 +34: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/views_slideshow/views_slideshow_plugin_style_slideshow.inc:
 +96: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +183: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +185: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +201: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +204: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/wysiwyg/wysiwyg.admin.inc:
 +141: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +143: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +153: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

modules/forum/forum.module:
 +744: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/field_group/field_group.field_ui.inc:
 +332: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/pathauto/pathauto.admin.inc:
 +27: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +36: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +54: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +202: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/pathauto/pathauto.inc:
 +588: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ip_geoloc/ip_geoloc.module:
 +840: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ip_geoloc/views/ip_geoloc_plugin_style.inc:
 +67: [critical] table names should be enclosed in {curly_brackets}
 +147: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +754: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +765: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ip_geoloc/views/ip_geoloc_plugin_style_leaflet.inc:
 +168: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +194: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +402: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +413: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +512: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +541: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ip_geoloc/views/ip_geoloc_plugin_style_map.inc:
 +81: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ip_geoloc/ip_geoloc_generator/ip_geoloc_generator.install:
 +12: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/ip_geoloc/ip_geoloc.admin.inc:
 +218: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/ip_geoloc/ip_geoloc.install:
 +12: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/ip_geoloc/ip_geoloc_api.inc:
 +88: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/modules/panels/panels_node/panels_node.module:
 +278: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/devel/devel.module:
 +450: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +1415: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +1864: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1885: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.

sites/all/modules/ctools/page_manager/plugins/tasks/page.admin.inc:
 +1316: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +1468: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/ctools/page_manager/page_manager.admin.inc:
 +1448: [critical] Potential problem: FAPI elements '#title' and '#description' only accept filtered text, be sure to use check_plain(), filter_xss() or similar to ensure your $variable is fully sanitized.
 +1512: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.
 +1669: [critical] Using eval() or drupal_eval() in your module's code could have a security risk if the PHP input provided to the function contains malicious code.

sites/all/modules/admin_menu/admin_menu.inc:
 +802: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +815: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.
 +900: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

sites/all/themes/denali_alaskan/inc/donationreq.php:
 +125: [critical] Use the Form API to build forms to help prevent against CSRF attacks.

sites/all/themes/denali_alaskan/inc/employmentapplication-backup.php:
 +478: [critical] Use the Form API to build forms to help prevent against CSRF attacks.

sites/all/themes/denali_alaskan/inc/employmentapplication-old.php:
 +769: [critical] Use the Form API to build forms to help prevent against CSRF attacks.

sites/all/themes/denali_alaskan/inc/employmentapplication.php:
 +9: [critical] table names should be enclosed in {curly_brackets}
 +790: [critical] Use the Form API to build forms to help prevent against CSRF attacks.

sites/all/themes/denali_alaskan/inc/joblistings-old.php:
 +8: [critical] table names should be enclosed in {curly_brackets}
 +40: [critical] table names should be enclosed in {curly_brackets}

sites/all/themes/denali_alaskan/inc/joblistings.php:
 +8: [critical] table names should be enclosed in {curly_brackets}
 +41: [critical] table names should be enclosed in {curly_brackets}

sites/all/themes/denali_alaskan/inc/rates.php:
 +4: [critical] table names should be enclosed in {curly_brackets}
 +10: [critical] table names should be enclosed in {curly_brackets}
 +20: [critical] table names should be enclosed in {curly_brackets}
 +27: [critical] table names should be enclosed in {curly_brackets}

sites/all/themes/zurb_foundation/theme-settings.php:
 +20: [critical] Potential problem: drupal_set_message() only accepts filtered text, be sure all !placeholders for $variables in t() are fully sanitized using check_plain(), filter_xss() or similar.

Status Messages:
 Coder found 239 projects, 2536 files, 269 critical warnings, 0 warnings were flagged to be ignored

```