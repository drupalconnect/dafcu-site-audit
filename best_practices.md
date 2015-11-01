# Best Practices

Below is a list of best practice items that should be addressed:

<div class="panel panel-danger"><div class="panel-heading"><strong>PHP Filter</strong><small> - Check if enabled.</small></div><p class="comments-section">PHP Filter is enabled! Executable code should never be stored in the database, and support for this feature was removed in Drupal 8 - https://drupal.org/node/1203886<div class="comments-icon"><div class="marker">+</div></div></p><div class="well well-small">Remove all executable code from your content and move it to your codebase.</div></div>