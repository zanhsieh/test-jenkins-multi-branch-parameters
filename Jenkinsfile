properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [
[$class: 'StringParameterDefinition', 
  name: 'base_tag',
  defaultValue: 'base-\${GIT_COMMIT}', 
  description: """For Docker b2b website project parent image name tag suffix assignment
                 |Syntax: base-[git commit] OR base-latest
                 |Example: base-A1B2C3 OR base-latest
                 |Default "base-\${GIT_COMMIT}" is for triggering via Github web hook""".stripMargin()], 
[$class: 'StringParameterDefinition', 
  name: 'names',
  defaultValue: 'dev-cn', 
  description: """For i18n specific region build
                 |Syntax: [environment1]-[region1],[environment2]-[region2],...,[environmentN]-[regionN]
                 |Example: dev-cn,dev-hk,prod-cn""".stripMargin()], 
[$class: 'StringParameterDefinition', 
  name: 'kube_version',
  defaultValue: '1.4.3', 
  description: """kubectl version. See: https://coreos.com/kubernetes/docs/latest/configure-kubectl.html
                 |Syntax: [number].[number].[number]
                 |Example: 1.4.3""".stripMargin()]]]]) 

node {
  stage ('Checkout') {
    echo "base_tag is ${base_tag}"
    echo "names is ${names}"
    echo "image_name is ${image_name}"
    echo "kube_version is ${kube_version}"
  }
}
