# Comandos Linux Essenciais para DevOps

Guia rápido com os comandos Linux mais usados por DevOps, SREs e administradores de sistemas.

### Foco
- Troubleshooting
- Monitoramento de logs
- Gerenciamento de serviços
- Permissões
- Automação e scripts

### Principais seções
1. Navegação (ls, cd, pwd)
2. Manipulação de arquivos/diretórios (mkdir, cp, mv, rm)
3. Visualização (cat, less, head, tail -f)
4. Busca e filtros (grep, awk, cut, wc)
5. Processos (ps, top/htop, kill)
6. Serviços systemd (systemctl, journalctl)
7. Permissões (chmod, chown)
8. Rede básica (ip, ping, curl, ss)
9. Disco e memória (df -h, free -h, du)

### Comandos curinga do dia a dia
```bash
ls -la
df -h
free -h
tail -f /var/log/*.log
journalctl -u serviço -f
grep -r "erro" /var/log/
ps aux | grep -i app
