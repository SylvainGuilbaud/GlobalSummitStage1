node {
    def app
    stage "Prepare environment"
        checkout scm
        app  = docker.build("widgetsdirect", "WidgetsDirect")

    stage "Test and validate"
        app.inside {
            sh "echo Testing..."
            //junit 'reports/**/*.xml'
        }
}