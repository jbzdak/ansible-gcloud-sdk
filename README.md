Role Name
=========

Downloads google cloud sdk and installs it to a directory 
of your choosing. 

I did not want to use package, as I dislike packages not 
maintained by debian team. 

Requirements
------------

All requirements are installed using apt.

Role Variables
--------------

Following object: 

     gcloud_sdk:
      add_to_path_for: []
      destination: "{{ extras_root }}/opt/gcloud-sdk"
      download:
        url: https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-155.0.0-linux-x86_64.tar.gz
        sha256: 4b64fba9d98b9e48cc7a37ed3b321e50f92e87f9c2b358d183f966dae05216a2
      dependencies:
        - python
