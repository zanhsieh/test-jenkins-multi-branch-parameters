properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [
[$class: 'StringParameterDefinition', 
  name: 'names',
  defaultValue: 'dev-cn', 
  description: """For i18n specific region build
                 |Syntax: [environment1]-[region1],[environment2]-[region2],...,[environmentN]-[regionN]
                 |Example: dev-cn,dev-hk,prod-cn""".stripMargin()], 
[$class: 'StringParameterDefinition', 
  name: 'image_name',
  defaultValue: 'gogotech/b2b-web', 
  description: """For Docker b2b website project parent image name tag prefix assignment
                 |Syntax: [organization name]/[which project]
                 |Example: gogotech/b2b-web""".stripMargin()], 
[$class: 'StringParameterDefinition', 
  name: 'kube_version',
  defaultValue: '1.4.3', 
  description: """kubectl version. See: https://coreos.com/kubernetes/docs/latest/configure-kubectl.html
                 |Syntax: [number].[number].[number]
                 |Example: 1.4.3""".stripMargin()]]]]) 

node {
  stage ('Checkout') {
    echo "image_name is ${image_name}"
    echo "kube_version is ${kube_version}"
  }
}
