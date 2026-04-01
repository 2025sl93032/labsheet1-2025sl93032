pipeline {
	agent any
	
	stages {
		stage('Checkout'){
		steps {
			git 'https://github.com/2025sl93032/labsheet1-2025sl93032.git'
}
}
		stage('Build'){
		steps {
		sh 'echo "Build stage running"'
}
}
		stage('Test'){
		steps {
			sh '''
			python3 -c "
			import calculator
			assert calculator.add(2,3)==5
			assert calculator.sub(5,3)==2
			print('All tests passed')
			"
			'''

}
}

		stage('Deploy'){
			steps {
				sh 'echo "Deploy stage(Dummy for now)'
}

}

}
}

