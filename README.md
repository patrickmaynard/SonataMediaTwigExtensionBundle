# Installation

1. Add the repository to the composer.json
```
#!yaml
...
"repositories": [
    {
      "type": "vcs",
      "url": "git@github.com:SocialbitGmbH/SonataMediaTwigExtensionBundle.git"
    }
  ],
...
```

2. Add composer requirement

```
#!sh
composer require socialbit/sonatamediatwigextension-bundle:~1.0
```

3. Add the bundle to the AppKernel

```
#!php
public function registerBundles()
{
    ...
    new Socialbit\\SonataMediaTwigExtensionBundle\SocialbitSonataMediaTwigExtensionBundle(),
    ...
}
```

4. Use the new helper in your twig templates: `{% set mediaUrl = media_public_url(media, 'reference') %}`

5. Enjoy