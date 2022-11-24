pipeline
{
    agent any
    parameters
    {
        string(defaultValue: "", description: "Profile Name", name: "Name")
        choice(choices: ["Male", "Female"], description: "Gender", name: "Gender")
        booleanParam(defaultValue: "false", description: "Confirm Details?", name: "Confirm")
    }
    stages
    {
        stage("Deploy")
        {
            steps
            {
                echo "Profile Number: ${env.BUILD_NUMBER} \n"
                echo "Name: ${params.Name} \n"
                echo "Gender: ${params.Gender} \n"
                echo "Confirm Details? : ${params.Confirm}"
            }
        }
    }
}