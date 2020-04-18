# Shopistry Private Composer

In order to use this repository you can add it using the `composer config repository.shopistry composer https://github.com/Shopistry/private-composer-repository.git`

To generate the repository, use the satis static composer repository generator. Pull the composer/satis docker image and then:

`docker run --rm --init -it   --user $(id -u):$(id -g)  --volume "$HOME/.composer:/composer"   --volume $(pwd):/build  composer/satis build satis.json .`

