# Домашнее задание к занятию "14.4 Сервис-аккаунты"

## Задача 1: Работа с сервис-аккаунтами через утилиту kubectl в установленном minikube

Выполните приведённые команды в консоли. Получите вывод команд. Сохраните
задачу 1 как справочный материал.

### Как создать сервис-аккаунт?

```
kubectl create serviceaccount netology
```

### Вывод команд

![Скриншот](img/Task1_1.png)

### Как просмотреть список сервис-акаунтов?

```
kubectl get serviceaccounts
kubectl get serviceaccount
```

### Вывод команд

![Скриншот](img/Task1_2.png)

### Как получить информацию в формате YAML и/или JSON?

```
kubectl get serviceaccount netology -o yaml
kubectl get serviceaccount default -o json
```

### Вывод команд

![Скриншот](img/Task1_3.png)

### Как выгрузить сервис-акаунты и сохранить его в файл?

```
kubectl get serviceaccounts -o json > serviceaccounts.json
kubectl get serviceaccount netology -o yaml > netology.yml
```
### Вывод команд

![Скриншот](img/Task1_4.png)

### Как удалить сервис-акаунт?

```
kubectl delete serviceaccount netology
```

### Вывод команд

![Скриншот](img/Task1_5.png)

### Как загрузить сервис-акаунт из файла?

```
kubectl apply -f netology.yml
```

### Вывод команд

![Скриншот](img/Task1_6.png)
