properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [
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
