# drush-monitor
Drush command to monitor Drupal updates.





actualys@sd-56006:/tmp/drupal-7.40$ grep -R _update_get_fetch_url_base .
./modules/update/update.fetch.inc:  $fetch_url_base = _update_get_fetch_url_base($project);
./modules/update/update.fetch.inc:  $url = _update_get_fetch_url_base($project);
./modules/update/update.fetch.inc:function _update_get_fetch_url_base($project) {
actualys@sd-56006:/tmp/drupal-7.40$ vi ./modules/update/update.fetch.inc
actualys@sd-56006:/tmp/drupal-7.40$ grep -R UPDATE_DEFAULT_URL .
./modules/update/update.fetch.inc:  return isset($project['info']['project status url']) ? $project['info']['project status url'] : variable_get('update_fetch_url', UPDATE_DEFAULT_URL);
./modules/update/update.module:define('UPDATE_DEFAULT_URL', 'http://updates.drupal.org/release-history');
