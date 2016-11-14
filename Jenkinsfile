properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [
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
  stage ('Checkout') {
    echo "image_name is ${image_name}"
    echo "kube_version is ${kube_version}"
  }
}
