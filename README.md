# Shopistry Private Composer

This repository has been generated with the Satis static composer repository generator. It is accessible at [https://shopistry.github.io/private-composer-repository/].

In order to use this repository you can add it using the `composer config repositories.shopistry composer https://shopistry.github.io/private-composer-repository/`

To generate the repository, use the satis static composer repository generator. Pull the composer/satis docker image and then:

`docker run --rm --init -it   --user $(id -u):$(id -g)  --volume "$HOME/.composer:/composer"   --volume $(pwd):/build  composer/satis build satis.json .`

To add a git repository as a project to this repository, edit the satis.json file and add another entry to the repositories object : 
`{ "type": "vcs", "url": "https://github.com/Shopistry/repo-name" }`
