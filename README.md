# amazee.io lagoon devsetup

Devsetup for amazee.io's lagoon based hosting.
Docs: https://lagoon.readthedocs.io/en/latest/

## Setup

  * Follow setup instructions from https://github.com/drunomics/devsetup-docker/tree/2.x

  * From your drupal-project root directory, run:

        git clone https://github.com/drunomics/devsetup-amazeeio devsetup-tmp
        rm -rf devsetup-tmp/.git devsetup-tmp/README.md
        cp -rfT devsetup-tmp devsetup-tmp .
            
        # Apply replacements and cleanup.
        php process-replacements.php
        rm -rf devsetup-tmp process-replacements.php

  * Then commit changes:
    
        git add .
        git commit -am "Added amazeeio lagoon support."
        
        
  * Follow lagoon docs for finishing the setup on amazeeio:

  https://lagoon.readthedocs.io/en/latest/using_lagoon/setup_project/#2-provide-access-to-your-code

## Credits

* Based upon the setup provided by amazee.io, see 
  https://github.com/amazeeio/drupal-example
* (c) 2018 drunomics GmbH, GNU GPLv2+
