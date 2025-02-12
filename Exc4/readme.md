# Спринт 7 задача 4

## Дисклеймер - похоже в задании ошибка. Либо требуется серьезное утонение.

Пользователи не создаются в minikube
Либо речь шла в задаче про ServiceAccount
Либо пользователи создаются с выпуском сертификатов
В материалах спринта ничего не сказано про создание пользователей. 
Зесь либо ошибка в требованиях, либо требуется учтоненние. 

Также, в задачнии сказано что нужно создать группы ролей, при этом в задании не сказано готовить файл....
они создаются:
kind: RoleBinding
apiVersion: rbac.authorization.k8s.io/v1
metadata:
  name: view-all-resources
subjects:
- kind: Group
  name: viewers
  apiGroup: rbac.authorization.k8s.io
roleRef:
  kind: Role
  name: viewer
  apiGroup: rbac.authorization.k8s.**io**