# sou-lab-cni
# Documentazione del Progetto

Questo progetto utilizza HAProxy come reverse proxy/load balancer per indirizzare le richieste a Grafana e Prometheus, entrambi eseguiti in container utilizzando Podman.

## Requisiti

- Ansible
- Vagrant

## Installazione

Eseguire il comando vagrant up per la creazione ed il provisioning delle VM sui due nodi.

(OPZIONALE) 
Aggiunta nel file /etc/hosts dei due hostname per testare direttamente da macchina host il corretto funzionamento del bilanciatore. 

192.168.50.11 grafana.local
192.168.50.11 prometheus.local

