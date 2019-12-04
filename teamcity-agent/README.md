
In order to configure additional runners, as out of the box the ["Kubernetes support" plugin](https://plugins.jetbrains.com/plugin/9818-kubernetes-support) does not support Docker or Gradle, I could not use a deployment pod template (error: image does not specify a 'source-id').  I ended up making my own deployment to customize the runners, though it's still more convenient to use the "Kubernetes support" plugin to authenticate the agents and dynamically scale them.

> 

This template under `spec` can be used in the plugin's "custom pod template", when creating a NEW image ONLY: + Add Image, Custom p od template.


