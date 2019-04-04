node {
    stage "checkout Code"
        git 'https://github.com/martinesmann/jenkins-ci-template.git'
    stage "Restore dependencies"
       bat label: '', script: 'nuget restore src\\MyWindowsService'
    stage "Build"
        bat label: '', script: 'src\\MyWindowsService\\MyWindowsService\\Deploy-Windows-Service-Via-MSBuild.proj'
}
