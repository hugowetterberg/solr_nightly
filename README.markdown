Solr 1.4.0
============

This is a set of convenience scripts for daily drupal use of solr in a dev environment.

Clone this repo and execute `get-nightly` from the terminal (when inside the solr_nightly directory) to download the latest nightly and set it up with the drupal-specific configuration files.

    $ ./get-nightly

Then execute `start` to get solr up and running. 

    $ ./start

Now your drupal install should be able to use solr. Press ctrl+c to quit solr. If you want to clear out all files that's been created for the search index and other runtime files (to use it with another drupal install, or just to start over), run:

    $ ./reset

Remember to delete the index from the drupal admin when you have a site that expects that there is a index. Otherwise your nodes won't be re-added.

Re-run the `get-nightly` script if you want to download the nightly again.