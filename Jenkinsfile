properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [
[$class: 'StringParameterDefinition', 
  defaultValue: 'base-\${GIT_COMMIT}', 
  description: """For Docker b2b website project parent image name tag suffix assignment
                 |Syntax: base-[git commit] OR base-latest
                 |Example: base-A1B2C3 OR base-latest
                 |Default "base-${GIT_COMMIT}" is for triggering via Github web hook""".stripMargin(), 
  name: 'base_tag'], 
[$class: 'StringParameterDefinition', 
  defaultValue: 'dev-cn', 
  description: """For i18n specific region build
                 |Syntax: [environment1]-[region1],[environment2]-[region2],...,[environmentN]-[regionN]
                 |Example: dev-cn,dev-hk,prod-cn""".stripMargin(), 
  name: 'names'],
[$class: 'StringParameterDefinition', 
  defaultValue: 'gogotech/b2b-web', 
  description: """For Docker b2b website project parent image name tag prefix assignment
                 |Syntax: [organization name]/[which project]
                 |Example: gogotech/b2b-web""".stripMargin(), 
  name: 'image_name'],
[$class: 'StringParameterDefinition', 
  defaultValue: '1.4.3', 
  description: """kubectl version. See: https://coreos.com/kubernetes/docs/latest/configure-kubectl.html
                 |Syntax: [number].[number].[number]
                 |Example: 1.4.3""".stripMargin(), 
  name: 'kube_version']]]])

node {
        // Mark the code checkout 'stage'....
        stage 'Checkout'
        // Get some code from a GitHub repository
}
