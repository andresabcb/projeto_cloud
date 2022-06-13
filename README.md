# Projeto Cloud - ABC Place

### Link do vídeo

https://alinsperedu.sharepoint.com/sites/Desa-Gravaodetrabalhos-GravaoDesa/Shared%20Documents/Recordings/New%20channel%20meeting-20220613_183828-Meeting%20Recording.mp4?web=1

### Terraform - Infraestrutura

Para aplicar os módulos eks e vpc:

```console
terraform init --upgrade
```

```console
terraform plan
```

```console
terraform apply
```

### Ansible - Aplicação

Para criar o deployment, expor o serviço e habilitar o autoscale:

```console
ansible-playbook playbook.yml -f 10
```

Para deletar o deployment e o serviço criados:

```console
ansible-playbook deletedeploy.yml -f 10
```

### Comandos úteis

Para conferir o que foi criado com o kubectl:

```console
kubectl get all
```

Para apagar algo que foi criado com o kubectl:

```console
kubectl delete <tipo_do_objeto/nome>
```
