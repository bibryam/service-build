# Custom OpenShift S2I build project to download artifacts from Nexus repo

The variables required by the build are as follows:

    NEXUS_URL - FQDN of the Nexus instance, e.g http://localhost:8081/
    REPOSITORY_NAME - id of the repo in Nexus e.g. snapshots
    GROUP_ID - e.g. com.demo.demo
    ARTIFACT_ID - e.g. demo
    ARTIFACT_VERSION - The version to pull from Nexus. Defaults to LATEST, but will accept RELEASE and snapshot versions (“1.0-SNAPSHOT”) as well.
    CLASSIFIER - The artifact type to pull. Defaults to app.
    EXTENSION - the extension of the artifact we want to retrieve. Defaults to zip.
