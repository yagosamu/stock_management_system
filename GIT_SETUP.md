# Comandos Git para Setup Inicial

## Para configurar o repositório pela primeira vez:

```bash
# Inicializar repositório Git
git init

# Adicionar origem remota
git remote add origin https://github.com/yagosamu/stock_management_system.git

# Configurar branch principal
git branch -M main

# Adicionar todos os arquivos
git add .

# Commit inicial
git commit -m "Initial commit: Stock Management System with Django"

# Push para o GitHub
git push -u origin main
```

## Para atualizações futuras:

```bash
# Adicionar mudanças
git add .

# Fazer commit das mudanças
git commit -m "Descrição das mudanças"

# Enviar para o GitHub
git push origin main
```

## Comandos úteis:

```bash
# Verificar status
git status

# Ver histórico
git log --oneline

# Ver arquivos modificados
git diff

# Verificar repositórios remotos
git remote -v
```