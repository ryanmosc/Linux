# Comandos Linux Essenciais para DevOps

Guia prático e organizado dos comandos mais usados no dia a dia de DevOps, SRE e SysAdmin.

---

## 1️⃣ Navegação em Diretórios e Arquivos

```bash
ls                  # lista arquivos e pastas do diretório atual
ls -l               # formato longo (permissões, dono, tamanho, data)
ls -la / ls -al     # formato longo + arquivos ocultos (.*)
ls -lh              # tamanhos em formato legível (K, M, G)
ls -l --sort=size   # ordena por tamanho (maior → menor)
```

```bash
cd ..               # sobe um nível
cd ../..            # sobe dois níveis
cd ~                # vai para o diretório home
cd -                # volta para o diretório anterior
pwd                 # mostra o caminho absoluto do diretório atual
```

---

## 2️⃣ Criação e Manipulação de Arquivos e Diretórios

```bash
mkdir projetos
mkdir -p caminho/completo/aninhado   # cria estrutura completa
```

```bash
cp arquivo.txt backup/
cp -r pasta/ destino/
cp -a pasta/ destino/                 # preserva permissões e datas (recomendado)
```

```bash
mv antigo.txt novo.txt                # renomeia arquivo
mv arquivo.txt /outro/local/          # move arquivo
mv pasta/ nova_pasta/                 # renomeia ou move diretório
```

```bash
rm arquivo.txt
rm -r pasta/
rm -rf pasta/                         # CUIDADO EXTREMO
```

---

## 3️⃣ Visualização de Conteúdo

```bash
cat arquivo.txt
cat -n arquivo.txt                    # numera linhas
less arquivo.log                      # visualização paginada
```

```bash
head -n 15 arquivo.txt
tail -n 30 arquivo.log
tail -f /var/log/nginx/access.log     # acompanhamento em tempo real
```

---

## 4️⃣ Busca, Filtros e Pipes

```bash
grep "erro" app.log
grep -i "error" *.log
grep -r "senha" /etc/
grep -v "DEBUG" app.log
ps aux | grep -i nginx
```

```bash
echo "texto" > arquivo.txt           # cria ou sobrescreve
echo "mais linha" >> arquivo.txt     # append
```

```bash
wc -l arquivo.log
cat acesso.log | wc -l
```

```bash
cut -d":" -f1 /etc/passwd
awk '{print $1, $9}' acesso.log
```

---

## 5️⃣ Processos

```bash
ps aux
ps aux | grep python
```

```bash
top
htop                                 # recomendado instalar
```

```bash
kill 1234                            # SIGTERM
kill -9 1234                         # SIGKILL
pkill -f "nome_processo"
killall nginx
```

---

## 6️⃣ Gerenciamento de Serviços (systemd)

```bash
systemctl status nginx
systemctl start nginx
systemctl restart nginx
systemctl stop nginx
systemctl enable nginx
systemctl disable nginx
systemctl reload nginx
```

```bash
journalctl -u nginx
journalctl -u nginx -n 100
journalctl -u nginx -f
journalctl -xe
```

---

## 7️⃣ Permissões e Proprietários

```bash
chmod 755 script.sh
chmod 644 arquivo.txt
chmod +x programa
chmod -R 755 public_html/
```

```bash
chown usuario arquivo.txt
chown usuario:desenvolvedores arquivo.txt
chown -R www-data:www-data /var/www/html
```

---

## 8️⃣ Rede (Básico)

```bash
ip a
ip a show eth0
```

```bash
ping 8.8.8.8
ping -c 4 google.com
```

```bash
curl https://api.exemplo.com
curl -I https://site.com
curl -s -o arquivo.zip https://download...
```

```bash
ss -tuln                            # portas TCP/UDP escutando
```

---

## 9️⃣ Disco, Memória e Sistema

```bash
df -h
df -h /var /home
```

```bash
free -h
```

```bash
du -sh pasta/
du -sh ./* | sort -hr
```

---

## 🔥 Recomendações Práticas para DevOps

Use com frequência:

* `ls -la`
* `df -h`
* `free -h`
* `journalctl -xe`
* `tail -f | grep`
* `ps aux | grep`

Esses comandos resolvem 80% dos problemas iniciais em produção.
