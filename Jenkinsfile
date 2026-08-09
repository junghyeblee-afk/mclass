pipeline {
    agent any // 어떤 에이전트(실행서버)에서든 실행 가능

    tools { // tools : Jenkins tools에 등록된 도구 사용.
        maven 'maven 3.9.12' // Jenkins Tools에 등록한 이름과 정확히 일치해야 함.
    }

    stages {    // Stage : 실제 자동 빌드를 수행하는 단계 정의.
        stage('Git Checkout'/*Git에 연결된 코드를 확인*/){ //수행 단계 구분
            steps { // 실제 수행할 명령어 정의.
                // Jenkins 가 연결된 Git 저장수에서 최신 코드 체크 아웃.
                checkout scm

            }

        }

    }
}