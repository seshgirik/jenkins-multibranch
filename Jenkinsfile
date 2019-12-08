node {

final REGITRY='registry.eng.hortonworks.com'

final BRANCH='stage'
final NAMESPACE='cdpe2e'
final DEFAULT_TAG='latest'
def tagName

stage('clone repo'){
def scmVars=checkout scm

//To handle git tags

branchName=scmVars.GIT_BRANCH.tokensize('/')[-1]

}

stage('build'){
println "docker buiild -f .qaas/Dockerfile.system_test -t ${REGISTRY}/${NAMESPACE}/cdpmc-qe-${BRANCH}:${tagName} ."
}

stage('cleanup'){
println "begin .. cleanpup"
}

}
