# pentaho-data-mining-subfloor
Subfloor support files for pdm build from Waikato repository
Moved from svn://source.pentaho.org/svnroot/pdm-subfloor

Additional files for PDM builds of Weka Waikato project
To build, you need to checkout Weka from a branch or tag here:
https://svn.cms.waikato.ac.nz/svn/weka/

Then clone/checkout a branch from this PDM subfloor project into the same path. This should create a subfloor project in the same folder with the Weka project.

Now run the ant build `clean-weka dist dist-source publish` with the typical property overrides:
-Divy.repository.publish=${PENTAHO_PUBLISH_REPOSITORY}
-Divy.repository.id=pentaho
-Dpentaho.resolve.repo=${PENTAHO_RESOLVE_REPO}
-Dproject.revision=${RELEASE_VERSION}
