# Release Notes

## 4.0.0 (Build - 2022112400)
Compatibility with Moodle 4.0
Remove errors and warnings from codechecker and phpdoc

## 3.8.0 (Build 2019112600)
Compatibility with Moodle 3.8 & 3.9
Updated subplugin declaration file to new subplugins.json structure.

## 3.3.0
An xpath change was required in the Behat tests in order to get Behat to pass due to changes in Moodle's output.

## 3.2
the plugin was rewritten to utilize the oembed provider definitions from [http://oembed.com/providers.json](http://oembed.com/providers.json).
The previous provider definitions that were hardcoded, but not present in the oembed provider list, were added as "local" definitions to avoid regression errors.

## 3.2.0.0 (Alpha)
Change highlights:

- Oembed providers defintions are downloaded from http://oembed.com/providers.json and stored in the Moodle database, rather than code.
- Oembed defintions are refreshed nightly with new additions and deletions.
- Management screen allows for administrators to save provider defintions as local overrides not refreshed by oembed.com.
- Two types of tags can be used for filtering. The one desired can be configured.
- Lazy loading can be turned on or off; default is on. This can improve site performance.
- Provider management screen allows enable/disable, and edit as local as well as providing all of the provider information.
- A subplugin system is in place to allow providers not stored at oembed.com to define oembed information.
  Some of the existing Microsoft providers have been rewritten as these.
