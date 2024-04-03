pipeline {
    agent any

    stages {
        stage('Load .env') {
            steps {
                script {
                    // อ่านไฟล์ .env และกำหนดค่าให้กับตัวแปร envMap
                    def envMap = readProperties file: '.env'

                    // ตั้งค่าตัวแปรสิ่งแวดล้อม BUILD_NUMBER จาก .env
                    env.BUILD_NUMBER_FROM_ENV = envMap['BUILD_NUMBER']

                    // แสดงค่า BUILD_NUMBER จาก .env
                    echo "BUILD_NUMBER from .env: ${env.BUILD_NUMBER_FROM_ENV}"
                }
            }
        }
    }
}
