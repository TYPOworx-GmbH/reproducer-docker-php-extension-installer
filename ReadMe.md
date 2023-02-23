# Reproducer for mlocati/docker-php-extension-installer
with Custom-Build to include PHP-Extensions

## Test cases
1. Dockerfile.test1
   Using scripted loop running ```install-php-extensions``` for each module separately
2. Dockerfile.test2
   Installing all modules in one RUN for ```install-php-extensions```
3. Dockerfile.test3
   Same as 2. but we're not manually extracting php-source (```docker-php-source extract```), showing this will result in build-errors
   during run for ```install-php-extensions```
