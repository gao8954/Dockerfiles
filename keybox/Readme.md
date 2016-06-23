keybox @ alpine linux (w/ OpenJRE)

---------------------

Build with [Dockerfile](https://github.com/jokester/Dockerfiles/blob/master/keybox/Dockerfile)

    # docker run -d --restart=always -v /persist/keybox-keydb:/keydb -p 8443:8443

Tomcat runs on port 8443

Places you may want to mount a volume with: `/artifactory-data/`. Because `{data,logs,backup,etc}` get symlinked to `/artifactory-oss/`
(see https://www.jfrog.com/confluence/display/RTF/Running+with+Docker#RunningwithDocker-RunningArtifactoryOSSorPro )
