# voting_app
Console Prints:
=~=~=~=~=~=~=~=~=~=~=~= PuTTY log 2022.09.05 12:55:03 =~=~=~=~=~=~=~=~=~=~=~=

[K[root@ip-172-31-1-221 k8s-specifications]# 
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# clear[Kclearkubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-7sfkt        1/1     Running   0          3m10s
redis-868d64d78-ndh4p     1/1     Running   0          5m13s
result-5d57b59f4b-v8lfd   1/1     Running   0          5m13s
vote-94849dc97-jgr9q      1/1     Running   0          4m39s
worker-dd46d7584-j8q8p    1/1     Running   1          4m20s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl delete all --all
pod "db-b54cd94f4-7sfkt" deleted
pod "redis-868d64d78-ndh4p" deleted
pod "result-5d57b59f4b-v8lfd" deleted
pod "vote-94849dc97-jgr9q" deleted
pod "worker-dd46d7584-j8q8p" deleted
service "db" deleted
service "kubernetes" deleted
service "redis" deleted
service "result" deleted
service "vote" deleted
deployment.apps "db" deleted
deployment.apps "redis" deleted
deployment.apps "result" deleted
deployment.apps "vote" deleted
deployment.apps "worker" deleted
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl delete all --all[10Pget po
No resources found in default namespace.
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get podelete all --all[10Pget po[9Pclearkubectl get podelete po db-b54cd94f4-jlwvrget po[Kdelete po worker-dd46d7584-6mhpjget po[Kdelete po vote-94849dc97-nxpr6get po[Kapply -f .[4Pget podelete all --all[10Pget po[9Pclearkubectl get po[9Pclearkubectl get podelete all --all[10Pget poapply -f .
deployment.apps/db created
service/db created
deployment.apps/redis created
service/redis created
deployment.apps/result created
service/result created
deployment.apps/vote created
service/vote created
deployment.apps/worker created
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl apply -f .[4Pget podelete all --all[10Pget po
NAME                      READY   STATUS              RESTARTS   AGE
db-b54cd94f4-dnjvd        1/1     Running             0          6s
redis-868d64d78-h9lmn     1/1     Running             0          6s
result-5d57b59f4b-6xtx8   1/1     Running             0          5s
vote-94849dc97-9gvc9      1/1     Running             0          5s
worker-dd46d7584-b45sv    0/1     ContainerCreating   0          5s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-dnjvd        1/1     Running   0          15s
redis-868d64d78-h9lmn     1/1     Running   0          15s
result-5d57b59f4b-6xtx8   1/1     Running   0          14s
vote-94849dc97-9gvc9      1/1     Running   0          14s
worker-dd46d7584-b45sv    1/1     Running   0          14s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl delete po vote-94849dc97-9gvc9
pod "vote-94849dc97-9gvc9" deleted
^C
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl delete po vote-94849dc97-9gvc9get po[K
NAME                      READY   STATUS              RESTARTS   AGE
db-b54cd94f4-dnjvd        1/1     Running             0          37s
redis-868d64d78-h9lmn     1/1     Running             0          37s
result-5d57b59f4b-6xtx8   1/1     Running             0          36s
vote-94849dc97-9gvc9      1/1     Terminating         0          36s
vote-94849dc97-zq79v      0/1     ContainerCreating   0          5s
worker-dd46d7584-b45sv    1/1     Running             0          36s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-dnjvd        1/1     Running   0          61s
redis-868d64d78-h9lmn     1/1     Running   0          61s
result-5d57b59f4b-6xtx8   1/1     Running   0          60s
vote-94849dc97-zq79v      1/1     Running   0          29s
worker-dd46d7584-b45sv    1/1     Running   0          60s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# 
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get podelete po vote-94849dc97-9gvc9[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[Kworker-dd46d7584-b45sv
pod "worker-dd46d7584-b45sv" deleted
^C
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl delete po worker-dd46d7584-b45svget po[K
NAME                      READY   STATUS              RESTARTS   AGE
db-b54cd94f4-dnjvd        1/1     Running             0          86s
redis-868d64d78-h9lmn     1/1     Running             0          86s
result-5d57b59f4b-6xtx8   1/1     Running             0          85s
vote-94849dc97-zq79v      1/1     Running             0          54s
worker-dd46d7584-b45sv    1/1     Terminating         0          85s
worker-dd46d7584-xsbnf    0/1     ContainerCreating   0          10s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS        RESTARTS   AGE
db-b54cd94f4-dnjvd        1/1     Running       0          99s
redis-868d64d78-h9lmn     1/1     Running       0          99s
result-5d57b59f4b-6xtx8   1/1     Running       0          98s
vote-94849dc97-zq79v      1/1     Running       0          67s
worker-dd46d7584-b45sv    1/1     Terminating   0          98s
worker-dd46d7584-xsbnf    1/1     Running       0          23s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-dnjvd        1/1     Running   0          118s
redis-868d64d78-h9lmn     1/1     Running   0          118s
result-5d57b59f4b-6xtx8   1/1     Running   0          117s
vote-94849dc97-zq79v      1/1     Running   0          86s
worker-dd46d7584-xsbnf    1/1     Running   0          42s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get podelete po worker-dd46d7584-b45sv[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[K[Kdb-b54cd94f4-dnjvd
pod "db-b54cd94f4-dnjvd" deleted
^C
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl delete po db-b54cd94f4-dnjvdget po[K
NAME                      READY   STATUS              RESTARTS   AGE
db-b54cd94f4-98mzz        0/1     ContainerCreating   0          3s
db-b54cd94f4-dnjvd        1/1     Terminating         0          2m16s
redis-868d64d78-h9lmn     1/1     Running             0          2m16s
result-5d57b59f4b-6xtx8   1/1     Running             0          2m15s
vote-94849dc97-zq79v      1/1     Running             0          104s
worker-dd46d7584-xsbnf    1/1     Running             0          60s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS        RESTARTS   AGE
db-b54cd94f4-98mzz        1/1     Running       0          16s
db-b54cd94f4-dnjvd        1/1     Terminating   0          2m29s
redis-868d64d78-h9lmn     1/1     Running       0          2m29s
result-5d57b59f4b-6xtx8   1/1     Running       0          2m28s
vote-94849dc97-zq79v      1/1     Running       0          117s
worker-dd46d7584-xsbnf    1/1     Running       0          73s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS        RESTARTS   AGE
db-b54cd94f4-98mzz        1/1     Running       0          25s
db-b54cd94f4-dnjvd        1/1     Terminating   0          2m38s
redis-868d64d78-h9lmn     1/1     Running       0          2m38s
result-5d57b59f4b-6xtx8   1/1     Running       0          2m37s
vote-94849dc97-zq79v      1/1     Running       0          2m6s
worker-dd46d7584-xsbnf    1/1     Running       0          82s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS        RESTARTS   AGE
db-b54cd94f4-98mzz        1/1     Running       0          34s
db-b54cd94f4-dnjvd        1/1     Terminating   0          2m47s
redis-868d64d78-h9lmn     1/1     Running       0          2m47s
result-5d57b59f4b-6xtx8   1/1     Running       0          2m46s
vote-94849dc97-zq79v      1/1     Running       0          2m15s
worker-dd46d7584-xsbnf    1/1     Running       0          91s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-98mzz        1/1     Running   0          44s
redis-868d64d78-h9lmn     1/1     Running   0          2m57s
result-5d57b59f4b-6xtx8   1/1     Running   0          2m56s
vote-94849dc97-zq79v      1/1     Running   0          2m25s
worker-dd46d7584-xsbnf    1/1     Running   1          101s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# 
[K[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-98mzz        1/1     Running   0          48s
redis-868d64d78-h9lmn     1/1     Running   0          3m1s
result-5d57b59f4b-6xtx8   1/1     Running   0          3m
vote-94849dc97-zq79v      1/1     Running   0          2m29s
worker-dd46d7584-xsbnf    1/1     Running   1          105s
]0;root@ip-172-31-1-221:~/example-voting-app/k8s-specifications[root@ip-172-31-1-221 k8s-specifications]# 

[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-98mzz        1/1     Running   0          8m26s
redis-868d64d78-h9lmn     1/1     Running   0          10m
result-5d57b59f4b-6xtx8   1/1     Running   0          10m
vote-94849dc97-zq79v      1/1     Running   0          10m
worker-dd46d7584-xsbnf    1/1     Running   1          9m23s
[root@ip-172-31-1-221 k8s-specifications]#
[root@ip-172-31-1-221 k8s-specifications]# kubectl delete all --all
pod "db-b54cd94f4-98mzz" deleted
pod "redis-868d64d78-h9lmn" deleted
pod "result-5d57b59f4b-6xtx8" deleted
pod "vote-94849dc97-zq79v" deleted
pod "worker-dd46d7584-xsbnf" deleted
service "db" deleted
service "kubernetes" deleted
service "redis" deleted
service "result" deleted
service "vote" deleted
deployment.apps "db" deleted
deployment.apps "redis" deleted
deployment.apps "result" deleted
deployment.apps "vote" deleted
deployment.apps "worker" deleted
[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
No resources found in default namespace.

[root@ip-172-31-1-221 k8s-specifications]# kubectl apply -f .
deployment.apps/db created
service/db created
deployment.apps/redis created
service/redis created
deployment.apps/result created
service/result created
deployment.apps/vote created
service/vote created
deployment.apps/worker created
[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS              RESTARTS   AGE
db-b54cd94f4-g42p4        0/1     ContainerCreating   0          5s
redis-868d64d78-c9vb8     0/1     ContainerCreating   0          5s
result-5d57b59f4b-rg27c   0/1     ContainerCreating   0          5s
vote-94849dc97-zdtkx      0/1     ContainerCreating   0          5s
worker-dd46d7584-rsvkt    0/1     ContainerCreating   0          5s
[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS              RESTARTS   AGE
db-b54cd94f4-g42p4        1/1     Running             0          20s
redis-868d64d78-c9vb8     0/1     ContainerCreating   0          20s
result-5d57b59f4b-rg27c   0/1     ContainerCreating   0          20s
vote-94849dc97-zdtkx      0/1     ContainerCreating   0          20s
worker-dd46d7584-rsvkt    0/1     ContainerCreating   0          20s
[root@ip-172-31-1-221 k8s-specifications]# kubectl get po
NAME                      READY   STATUS    RESTARTS   AGE
db-b54cd94f4-g42p4        1/1     Running   0          57s
redis-868d64d78-c9vb8     1/1     Running   0          57s
result-5d57b59f4b-rg27c   1/1     Running   0          57s
vote-94849dc97-zdtkx      1/1     Running   0          57s
worker-dd46d7584-rsvkt    1/1     Running   0          57s
[root@ip-172-31-1-221 k8s-specifications]#


--------------------------------------------------------------------

Observations: 
1. After deleting Voting Pod, the pod got recreated and there was no effect on the app. Cross checked with manual voting.
2. After deleting Worker Pod, the pod got created and there was no effect on the app. Cross checked with manual voting.
3. After deleting db Pod, the pod got created. But the Voting app in the browsed misbehaved. The results were not correct. 
4. After deleting all the pods and re-creating, the app started working fine.
