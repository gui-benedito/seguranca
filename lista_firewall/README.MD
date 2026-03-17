# UFW vs IPTABLES - Script de Firewall

Script em Bash para gerenciamento de firewall usando UFW e iptables.

---

## Objetivo

Comparar e praticar comandos de:

- UFW (alto nível)
- iptables (baixo nível)

---

## Pré-requisitos

- Linux (Ubuntu recomendado)
- Bash
- UFW
- iptables

Instalação:

```bash
sudo apt update
sudo apt install ufw iptables -y
```

---

## Execução

Dar permissão:

```bash
chmod +x exercicios_firewall
```

Executar:

```bash
sudo ./exercicios_firewall
```

---

## Uso

Ao executar, será exibido um menu:

```
1  - Verificar status
2  - Habilitar UFW
3  - Desabilitar UFW
...
22 - NAT 80 -> 8080
0  - Sair
```

Digite o número da opção e pressione ENTER.

---

## Observações

- O script precisa de sudo
- UFW e iptables são usados juntos apenas para estudo
- Em produção, normalmente se usa apenas um

---

## Permissão sem senha (opcional)

Editar sudoers:

```bash
sudo visudo
```

Adicionar:

```
seu_usuario ALL=(ALL) NOPASSWD: /usr/sbin/ufw, /usr/sbin/iptables
```
