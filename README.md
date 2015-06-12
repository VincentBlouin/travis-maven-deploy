This repo contains a `settings.xml` file that can be used to deploy snapshots to SonaType from a
Travis CI build. The full instructions are here:

http://xeiam.com/configure-travis-ci-to-deploy-snapshots/

Note: For the travis.yml you can simply use "git clone https://github.com/VincentBlouin/travis-maven-deploy.git target/travis" and remove `git config --get remote.origin.url`. Also in the script &amp;&amp; mvn clean deploy replace  &amp;&amp; by &&

That article recommends putting these settings in a branch in your project, but having it in a new
project avoids cloning your entire (possibly large) Git repo just for one settings file.
