properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [
[$class: 'StringParameterDefinition', 
  defaultValue: '1.4.3', 
  description: """kubectl version. See: https://coreos.com/kubernetes/docs/latest/configure-kubectl.html
                 |Syntax: [number].[number].[number]
                 |Example: 1.4.3""".stripMargin(), 
  name: 'kube_version']]]])

node {
  stage ('Checkout') {
    echo "kube_version is ${kube_version}"
  }
}
