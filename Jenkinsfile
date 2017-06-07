node('android') {
  stage 'Checkout'
	checkout scm

	stage 'Prepare'
	sh 'ls $HOME/.jenkins'
	sh 'env'
	sh 'id'
	sh 'ls /opt/nvm'
	sh 'cordova platform add android'
	sh 'cordova prepare android'

	stage 'Build'
	sh 'cordova build android'

	stage 'Archive'
	println('Done!')
}
