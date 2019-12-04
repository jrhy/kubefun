
In order to configure additional runners, as out of the box the ["Kubernetes support" plugin](https://plugins.jetbrains.com/plugin/9818-kubernetes-support) does not support Docker or Gradle, I could not use a deployment pod template (error: image does not specify a 'source-id').  I ended up making my own deployment to customize the runners, obviating the reason to use the "Kubernetes support" plugin.

> 

This is my template for adding additional runners.

