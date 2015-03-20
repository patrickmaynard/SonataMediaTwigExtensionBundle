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


## License  
    Copyright 2014 Socialbit GmbH

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.   
