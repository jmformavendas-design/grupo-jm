# 📁 Projeto Grupo JM

## 📋 Estrutura do Projeto


Vou criar um README completo com a estrutura e instruções para setup. Primeiro, vou criar o arquivo:

## 📝 **CRIANDO README.md COMPLETO:**

```bash
cd ~/grupo-jm
cat > README.md << 'EOF'
# 📁 Projeto Grupo JM

## 📋 Estrutura do Projeto

```
grupo-jm/
├── README.md          # Este arquivo
├── companies/         # Diretório de empresas
│   ├── jm-forma/      # Arquivos JM Forma
│   │   └── README.md  # Documentação JM Forma
│   └── jm-personalizados/  # Arquivos JM Personalizados
│       └── README.md  # Documentação JM Personalizados
├── imagens/           # Diretório de imagens
│   └── teste          # Arquivo de exemplo
└── teste              # Arquivo de teste
```

## 🚀 Setup para Desenvolvimento (WSL/Ubuntu)

### Pré-requisitos
- Git instalado
- WSL2 configurado (se for Windows)
- Acesso ao repositório GitHub

### Passo 1: Clonar o Repositório
```bash
# Clone o projeto
git clone https://github.com/jmformavendas-design/grupo-jm.git

# Entre na pasta do projeto
cd grupo-jm
```

### Passo 2: Configurar Git (primeira vez)
```bash
# Configurar usuário (substitua com seus dados)
git config user.name "Seu Nome"
git config user.email "seu.email@exemplo.com"

# Verificar configuração
git config --list
```

### Passo 3: Trabalhar com Branches

#### Ver branches disponíveis:
```bash
git branch -a
```

#### Mudar para uma branch:
```bash
git checkout nome-da-branch
# Exemplo:
git checkout teste_rayan
git checkout teste_luiz
git checkout main
```

#### Criar nova branch para desenvolver:
```bash
git checkout -b minha-nova-feature
```

### Passo 4: Fluxo de Trabalho

1. **Atualize sua branch:**
```bash
git pull origin nome-da-branch
```

2. **Faça suas alterações...**

3. **Adicione arquivos modificados:**
```bash
git add .
# Ou arquivos específicos
git add caminho/do/arquivo
```

4. **Commit suas mudanças:**
```bash
git commit -m "Descrição clara das alterações"
```

5. **Envie para o GitHub:**
```bash
git push origin nome-da-branch
```

## 🌿 Branches Principais

- **`main`** - Branch de produção (estável)
- **`teste_rayan`** - Branch de testes do Rayan
- **`teste_luiz`** - Branch de testes do Luiz

## 📁 Convenções de Pastas

- `companies/` - Documentos e arquivos relacionados às empresas
- `imagens/` - Imagens e assets visuais do projeto
- Cada subpasta deve conter um `README.md` explicando seu conteúdo

## 🔗 URLs Úteis

- **Repositório GitHub:** https://github.com/jmformavendas-design/grupo-jm
- **Branch main:** https://github.com/jmformavendas-design/grupo-jm/tree/main
- **Branch teste_rayan:** https://github.com/jmformavendas-design/grupo-jm/tree/teste_rayan
- **Branch teste_luiz:** https://github.com/jmformavendas-design/grupo-jm/tree/teste_luiz

## ⚠️ Notas Importantes

1. **Pastas vazias** não são commitadas no Git. Se uma pasta precisa existir, adicione um arquivo `.gitkeep` ou `README.md` dentro dela.

2. **Sempre faça pull antes de push** para evitar conflitos.

3. **Use mensagens de commit descritivas**.

4. **Mantenha seu .gitignore atualizado** para não commit arquivos desnecessários.

## 🆘 Troubleshooting

### Erro "Permission denied"
```bash
# Verificar permissões
git remote -v

# Se usar token, configurar:
git remote set-url origin https://usuario:token@github.com/jmformavendas-design/grupo-jm.git
```

### Pastas não aparecendo
```bash
# Se pastas vazias não aparecem, adicione um arquivo:
touch nome-da-pasta/.gitkeep
git add nome-da-pasta/
git commit -m "Adiciona pasta vazia"
```

---

**Desenvolvido por:** Equipe Grupo JM  
**Última atualização:** $(date +"%d/%m/%Y")
