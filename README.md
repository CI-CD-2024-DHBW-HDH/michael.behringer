# Michael Behringer Aufgabe 5

## Welche Vorteile ein Kubernetes Deployment gegenüber einem Kubernetes Pod hat **(2 Punkte)**
Ein Pod ist die kleinste Einheit in Kubernetes, ein Kubernetes Deployment verwaltet mehrerer Pods.
- Anzahl der Pods können einfach skaliert werden.
- Es sind Rolling Updates möglich.
- Rollbacks auf frühere Versionen.
- Automatisches Neustarten Von Pods.
## Wofür ein Kubernetes Service gut ist **(2 Punkte)**
Ein Service kann Pods, Deployments usw. in einem Cluster im Netzwerk innerhalb und auserhalb erreichbar machen, Services bieten eine konstante IP-Adresse. Ein Service verteilt Anfragen automatisch auf alle Pods, die zu einem bestimmten Service gehören, und fungiert somit als einfacher Lastverteiler.
## Mehrere Wege wie man eine Kubernetes Anwendung von außen erreichen kann **(3 Punkte)**
- NodePort: Ein NodePort-Service macht eine Anwendung zugänglich, indem für jeden Node im Cluster ein spezifischer Port geöffnet wird
- LoadBalancer: Bei Cloud-basierten Kubernetes-Installationen kann ein LoadBalancer-Service verwendet werden, der einen externen Load Balancer mit einer öffentlichen IP-Adresse bereitstellt.
- Ingress: Über ein Ingress Controller kann über eine einzige IP-Adresse von außen auf das Cluster zugegriffen werden.
