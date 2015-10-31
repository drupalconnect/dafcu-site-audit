# Location Patch

```
diff -uprb a/contrib/location_cck/location_cck.module b/contrib/location_cck/location_cck.module
--- contrib/location_cck/location_cck.module	2013-10-30 11:35:12.000000000 -0600
+++ contrib/location_cck/location_cck.module	2015-10-13 09:43:14.000000000 -0600
@@ -617,7 +617,7 @@ function location_cck_tokens($type, $tok
     // Loop through the tokens.
     foreach ($tokens as $name => $original) {
       // Break our token into an array to use later.
-      $fields = explode(':', $name);
+      $fields = explode(':', str_replace(array('[', ']'), '', $original));
       $entity = $fields[0];
       $field = $fields[1];
       // Allow for a position at the end of the token. If no position is given
@@ -625,7 +625,7 @@ function location_cck_tokens($type, $tok
       $position = (isset($fields[2]) && is_numeric($fields[2]) ? $fields[2] : 0);

       // If the token is in the $available, replace it.
-      if($available[$field]) {
+      if(array_key_exists($field, $available) && $available[$field]) {
         $replacements[$original] = (isset($node->{$entity}[LANGUAGE_NONE][$position][$field]) ? $node->{$entity}[LANGUAGE_NONE][$position][$field] : '');
       }
     }
Only in /Users/tommy/devdesktop/dafcu/sites/all/modules/location/: sniffers.sh
```