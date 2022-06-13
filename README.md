# Projeto Cloud - ABC Place

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
ansible-playbook deletepods.yml -f 10
```

### Comandos úteis

Para conferir o que foi criado com o kubectl:

```console
kubectl get all
```
