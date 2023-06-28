## OTUS Administrator Linux. Professional ДЗ №22: DNS-настройка и обслуживание

**Задание**

Для выполнения домашнего задания используйте методичку
https://docs.google.com/document/d/13kjusaFEzv6Ip_9soeDj2Ry-6WK8IDX7/edit?usp=share_link&ouid=104106368295333385634&rtpof=true&sd=true

1. взять стенд https://github.com/erlong15/vagrant-bind [скопировано](./vagrant-bind)
2. добавить еще один сервер client2
3. завести в зоне dns.lab имена

- web1 - смотрит на клиент1
- web2 смотрит на клиент2

4. завести еще одну зону newdns.lab
5. завести в ней запись

- www - смотрит на обоих клиентов

6. настроить split-dns:

- клиент1 - видит обе зоны, но в зоне dns.lab только web1
- клиент2 видит только dns.lab

7. (\*) настроить все без выключения selinux

Формат сдачи: Vagrantfile + ansible

**_Решение_**
