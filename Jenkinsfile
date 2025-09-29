@Library(['FPAC-Standard'])_
FpacPipeline {
    isRelease = false
    sourcePath = './'
    testPath = './'
    nodeJSInstallationName = 'NodeJS-22-LTS'

    doPrepare = { pipeline,settings ->
        pipeline.echo "Sample Prepare Stage for ${settings.ProjectName()}"
    }

    doBuild = { pipeline, settings ->
        pipeline.nodejs(configId: 'FsaNpmrc', nodeJSInstallationName: 'NodeJS-22-LTS') {
            sh 'npm install --no-audit'
            sh 'npm run build'
        }
    }

    doPackage = { pipeline,settings ->
        pipeline.nodejs(configId: 'FsaNpmrc', nodeJSInstallationName: 'NodeJS-22-LTS') {
            sh 'cp package.json dist'
        }
    }

    doPreValidate = { pipeline,settings ->
        pipeline.echo "Sample Pre Validate Stage for ${settings.ProjectName()}"
    }

    components = [
        NpmComponent([sourcePath:'./src'], 'Sample Application Frontend', './dist', './')
    ]
}