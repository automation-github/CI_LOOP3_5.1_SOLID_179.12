pipeline {
  agent any
  stages {
    stage('	resiliency_with_machine_groups_npvr_5.1') {
      agent any
      environment {
        target_cluster = '10.65.179.12'
        test_name = 'test_ingest_resilency_npvr.py'
      }
      steps {
        build '	resiliency_with_machine_groups_npvr_5.1'
      }
    }
    stage('resiliency_with_machine_groups_rb_5.1') {
      agent any
      environment {
        target_cluster = '10.65.179.12'
        test_name = 'test_ingest_resilency_rb.py'
      }
      steps {
        build 'resiliency_with_machine_groups_rb_5.1'
      }
    }
  }
}